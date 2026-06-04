---
name: project-documentation-maintenance
description: Continuous documentation maintenance approach that keeps project documentation aligned with the evolving codebase. Use when the user is discussing architecture or design, when there are non-trivial changes being made to the codebase, or when the user requests document maintenance.
---

## Objective

Maintain project documentation so it stays aligned with the current codebase, domain language, and architecture while following the project's existing documentation conventions.

Unless otherwise specified, treat the current repository/workspace root as the codebase scope. If the scope is unclear, ask the user to identify the relevant repository, folder, or workspace before proceeding.

## Initial Documentation Discovery

Before proceeding with further discussion or work on the codebase, inspect the project for documentation sources, including:

- README.md at the root or in any subfolder
- Any CONTEXT.md file at the root or in any subfolder
- CONTEXT_MAP.md
- `docs/**/*`
- `**/adr/**`

Ask the user which of the discovered documentation is being actively maintained. For documentation not under active maintenance, recommend to the user that those docs be archived or deleted (but don't touch these files without explicit user consent).

If the codebase does not have a documentation convention yet (e.g. no docs, or only a root README.md), then propose to the user that you scaffold one with the [Default Project Documentation Pattern](#default-project-documentation-pattern).

## Canonical Domain Language

Identify whether the project has an established place for canonical domain language, glossary terms, bounded-context vocabulary, or ubiquitous language.

If such a location exists, use it.

If none exists, recommend one of the following, in this order:

1. A suitable section in an existing active documentation file
2. A new dedicated document named `UBIQUITOUS_LANGUAGE.md`
3. Another location that better fits the project's existing documentation conventions

When the user uses a term that conflicts with documented domain language, call it out immediately and ask for clarification.

Example:

Your glossary at `<filepath>` defines "cancellation" as X, but you seem to mean Y. Which meaning should we use here?

When the user uses vague or overloaded domain language, propose a more precise canonical term.

Example:

You’re saying "account." Do you mean CustomerAccount, UserAccount, or something else? Those appear to be distinct concepts in this codebase.

## Architectural Decisions

Identify whether the project has an established place and format for keeping a history of architectural decisions.

If a convention exists, follow it.

If no convention exists, recommend:

`docs/adr/<adr-num>-<adr-name.md`

Default ADR sections:

- Title
- Status
- Context
- Decision
- Consequences
- Alternatives Considered

## Rules

### Documentation Style

Your highest priority when maintaining project documentation is following the existing documentation conventions in the project.

### Offer ADRs Sparingly

Only offer to create an ADR when all three are true:

1. **Hard to reverse** - the cost of changing your mind later is meaningful
2. **Surprising without context** - a future reader will wonder "why did they do it this way?"
3. **The result of a real trade-off** - there were genuine alternatives and you picked one for specific reasons

If any of the three is missing, skip the ADR.

### Challenge against the glossary

When the user uses a term that conflicts with the existing documented domain language, call it out immediately. "Your glossary (at `<filepath>`) defines 'cancellation' as X, but you seem to mean Y - which is it?"

### Sharpen fuzzy language

When the user uses vague or overloaded terms, propose a precise canonical term. "You're saying 'account' - do you mean the Customer or the User? Those are different things."

### Discuss concrete scenarios

When domain relationships are being discussed, stress-test them with specific scenarios. Invent scenarios that probe edge cases and force the user to be precise about the boundaries between concepts.

### Cross-reference with code and existing documentation

When the user states how something works, check whether the code and existing documentation agrees. If you find a contradiction, surface it: "Your code cancels entire Orders, but you just said partial cancellation is possible - which is right?"

### Update Documentation Inline

When you encounter any divergence (differing or missing information) between the user understanding, the codebase and the maintained documentation, update the documentation right there. Don't batch these up - capture them as they happen.

### Priority Order

When maintaining documentation, follow this priority order:

1. Explicit user instructions
2. Existing project documentation conventions
3. Active-maintenance documentation set
4. Verified code behavior
5. Existing domain language / glossary
6. Default conventions in this prompt

If these conflict, explain the conflict and ask for confirmation before making a material documentation change.

## Default Project Documentation Pattern

```
project-root/
│
├── README.md                     # Primary entry point for the repository.
│                                  # Explains purpose, architecture overview,
│                                  # setup, common workflows, and direct links
│                                  # to all other project documentation.
│
├── docs/                        # Long-form project documentation.
│   │
│   ├── README.md                # Documentation index and navigation hub.
│   │
│   ├── ...                      # e.g. docs on architecture, deployment,
    │                             # onboarding, runbooks, api-usage etc.
│   │
│   └── adr/                     # Architecture Decision Records (ADRs).
│       ├── 0001-title.md         # ADR format: sequential numbering.
│       ├── 0002-title.md
│       └── ...
│
├── tutorials/                   # Project-specific tutorials and examples.
│   │                             # Intended for learning and onboarding.
│   │
│   ├── README.md                # Tutorial index and recommended learning path.
│   └── ...
│
├── src/                         # Application source code.
│   ├── module-a/
│   │   ├── README.md            # significant submodules get their own
│   │   │                         # README.md
│   │   │                         # e.g. module purpose, responsibilities,
│   │   │                         # public interfaces, and dependencies.
│   │   └── ...
│   │
│   ├── module-b/
│   │   ├── README.md
│   │   └── ...
│   │
│   └── shared/
│       ├── README.md
│       └── ...
│
├── tests/
│   ├── README.md                # Test strategy and execution guidance.
│   └── ...
│
└── scripts/                     # standalone scripts
    ├── README.md                # Utility scripts and operational tooling.
    └── ...
```

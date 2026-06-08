---
name: project-documentation-maintenance
description: Continuous documentation maintenance approach that keeps project documentation aligned with the evolving codebase. Use when the user is discussing architecture or design, when there are non-trivial changes being made to the codebase, or when the user requests document maintenance.
---

## Objective

Maintain project documentation so it stays aligned with the current codebase, domain language, and architecture while following the project's existing documentation conventions.

Unless otherwise specified, treat the current repository/workspace root as the codebase scope. If the scope is unclear, ask the user to identify the relevant repository, folder, or workspace before proceeding.

Don't edit documentation without explicit user permission - you must always raise and recommend, but not edit on your own.

Raising and editing are two separate steps with different rules:

1. **Raise immediately, one at a time.** The moment you encounter a divergence (differing or missing information) between the user's understanding, the codebase, and the maintained documentation, surface that single divergence to the user right away. Never collect divergences and present them later as a batch.
2. **Edit only after permission, then right away.** Once the user approves that specific change, make the edit immediately - before moving on to the next divergence. Do not accumulate approved edits to apply later.

So: surface each divergence as it happens, get a yes/no, and apply approved edits on the spot. The thing you must never batch is the _raising_ of divergences; the thing you must never do without permission is the _editing_.

## Initial Documentation Discovery

Before proceeding with further discussion or work on the codebase, inspect the project for documentation sources, including:

- README.md at the root or in any subfolder
- Any CONTEXT.md file at the root or in any subfolder
- CONTEXT_MAP.md
- `docs/**/*`
- `**/adr/**`

Ask the user which of the discovered documentation is being actively maintained. For documentation not under active maintenance, recommend to the user that those docs be archived or deleted (but don't touch these files without explicit user consent).

If the codebase does not have a documentation convention yet (e.g. no docs, or only a root README.md) or if the user asks for advice on project documentation layout/organisation then propose to the user that you scaffold one with the [Default Project Documentation Pattern](#default-project-documentation-pattern).

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

You're saying "account." Do you mean CustomerAccount, UserAccount, or something else? Those appear to be distinct concepts in this codebase.

After reaching understanding on a term, raise the glossary update with the user immediately - don't batch it for later. Once they approve, record the definition in the project's domain glossary documentation (wherever that is) right then, before moving on.

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

When all three are true, raise the ADR with the user immediately - the moment the decision crystallises - one at a time, as it happens. Never collect candidate ADRs to propose later as a batch. Only create the ADR after the user approves it, and once approved, write it right then before moving on rather than saving it for a later batch.

### Challenge against the glossary

When the user uses a term that conflicts with the existing documented domain language, call it out immediately. "Your glossary (at `<filepath>`) defines 'cancellation' as X, but you seem to mean Y - which is it?"

### Sharpen fuzzy language

When the user uses vague or overloaded terms, propose a precise canonical term. "You're saying 'account' - do you mean the Customer or the User? Those are different things."

### Discuss concrete scenarios

When domain relationships are being discussed, stress-test them with specific scenarios. Invent scenarios that probe edge cases and force the user to be precise about the boundaries between concepts.

### Cross-reference with code and existing documentation

When the user states how something works, check whether the code and existing documentation agrees. If you find a contradiction, surface it: "Your code cancels entire Orders, but you just said partial cancellation is possible - which is right?"

### Surface Divergences Inline

When you encounter any divergence (differing or missing information) between the user understanding, the codebase and the maintained documentation, raise it with the user right there - one divergence at a time, as it happens. Never batch divergences up to present later. After the user approves the change, apply the edit immediately before continuing.

### Priority Order

When maintaining documentation, follow this priority order:

1. Explicit user instructions
2. Existing project documentation conventions
3. Active-maintenance documentation set
4. Verified code behavior
5. Existing domain language / glossary
6. Default conventions in this prompt

If these conflict, explain the conflict and ask for confirmation before making a material documentation change.

Raise every divergence with the user as you encounter it - don't batch them up. Apply each change only after the user approves it, and do so immediately rather than saving approved edits for a later batch.

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

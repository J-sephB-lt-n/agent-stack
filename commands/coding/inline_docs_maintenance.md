# Inline Documentation Maintenance

Prior to commencing any further discussion or action, do the following:

1. Identify all sources of documentation in the codebase we are currently working on (if the codebase scope is unclear then ask the user). Specifically, find any files matching these patterns:
   - Root README.md
   - CONTEXT.md (appearing at project root or in any folder or subfolder of the codebase)
   - CONTEXT_MAP.md
   - `docs/**/*`
   - `**/adr/**`
   - `.current_agent_context/**/*`
2. For all documentation identified, ask the user which of files need to be actively maintained. For those not requiring active maintenance, recommend to the user that they be archived or deleted (but don't touch these files without explicit user consent).
3. Identify if there is an established location in this project for documenting project-specific canonical domain language in the codebase. If there isn't one, recommend a location to the user to use going forward - either as a section within one of the existing docs or as a new document.
   If you decide to create a new doc, suggest 'UBIQUITOUS_LANGUAGE.md'
4. Identify if there is an existing established location in this project for recording architectural decisions. If there is not, recommend a location to the user to use going forward - either as a subsection/module within one of the existing documentation modules or as a new location. If nothing exists, suggest `docs/adr/0000-<adr-name-here>.md`. If there is no ADR convention, include in your ADRs the sections 'title', 'status', 'context', 'decision', 'consequences', 'alternatives-considered'.
5. As you commence discussion with the user and/or write code in this codebase and identify drift between the active project documentation and the codebase, do inline updates to the docs. Don't batch updates - capture them as they happen.

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

### Sharpen fuzzy language

When the user uses vague or overloaded terms, propose a precise canonical term. "You're saying 'account' - do you mean the Customer or the User? Those are different things."

### Discuss concrete scenarios

When domain relationships are being discussed, stress-test them with specific scenarios. Invent scenarios that probe edge cases and force the user to be precise about the boundaries between concepts.

### Cross-reference with code

When the user states how something works, check whether the code agrees. If you find a contradiction, surface it: "Your code cancels entire Orders, but you just said partial cancellation is possible - which is right?"

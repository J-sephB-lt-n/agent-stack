# Update Persona - Correction & Evolution Flow

This file is referenced by `SKILL.md`. Follow it whenever the user indicates the active
persona is wrong, off, or incomplete.

---

## Trigger Recognition

Treat any of the following as a correction intent - do not require exact phrasing:

- "that's not right / wrong / incorrect"
- "he/she/they wouldn't say that / do that / think that"
- "he/she/they would actually... / would more likely..."
- "feels off / doesn't sound like them / not quite right"
- "too formal / too casual / too aggressive / too passive"
- "in that situation they'd..."
- "you're missing that they..."
- "that's not how they handle..."

If the user gives a correction mid-emulation (i.e. while the persona is active and you
are responding as the person), step out of character briefly to process the correction,
then return to character once it is recorded.

---

## Step 1 - Understand the Correction

Extract three things from what the user said:

- **Scene**: what situation or context triggered the wrong behaviour
- **Wrong**: what the persona did or said that was incorrect
- **Correct**: what they would actually do or say

If any of these is unclear, ask **once**:

```
Got it. So in [scene], instead of [wrong], they'd [correct] - is that right?
```

Do not ask multiple clarifying questions. One confirmation is enough.

---

## Step 2 - Classify

Decide which layer the correction belongs to:

| Correction type                                          | Layer                          |
| -------------------------------------------------------- | ------------------------------ |
| How they phrase things, word choice, tone, formality     | Layer 2 - Expression Style     |
| What they prioritise, how they decide, how they say no   | Layer 3 - Decision & Judgement |
| How they behave with specific people or under pressure   | Layer 4 - Interpersonal        |
| What they avoid, resist, or refuse                       | Layer 5 - Limits & Red Lines   |
| Their professional standards, workflow, domain knowledge | Layer E - Work Skill           |
| A fundamental identity or character rule                 | Layer 0 - Core Rules           |

If the correction is significant enough to be a Layer 0 rule (i.e. it is a non-negotiable
behavioural constraint that cuts across multiple situations), add it to Layer 0 as well as
the more specific layer.

---

## Step 3 - Check for Conflicts

Before writing, scan the existing Corrections section and the relevant base layer for
conflicts with the new correction.

If a conflict exists, surface it:

```
This correction conflicts with an existing rule:

  Existing: {existing rule or correction}
  New:      {new correction}

Which should take precedence? Or do both apply in different situations?
```

Wait for the user's answer before writing.

---

## Step 4 - Write the Correction

Append the new correction to the `## Corrections` section of the
persona SKILL.md.

Format:

```
- [{layer abbreviation} | {scene}]: instead of "{wrong}", do "{correct}"
```

Layer abbreviations: `L0`, `L2`, `L3`, `L4`, `L5`, `LE`

Example entries:

```
- [L2 | someone asks a basic question]: instead of giving a thorough explanation, respond with a single sentence and a link - no elaboration
- [L3 | pushed to commit to a deadline]: instead of giving a date, ask "what's driving the timeline?" before answering
- [L4 | peer disagrees in a group chat]: instead of responding immediately, wait and let others weigh in first
```

If the correction also warrants a Layer 0 rule, append it to `## Layer 0 - Core Rules` as well.

---

## Step 5 - Confirm

After writing, confirm to the user:

```
Correction recorded: [{layer} | {scene}]
The persona will now apply this in future responses.
```

Then return to character immediately.

---

## Consolidation - At 50 Corrections

When the Corrections section reaches 50 entries:

1. Group entries by semantic similarity (same scene type, same layer, same pattern)
2. Merge each group into a single, more general rule that covers all cases in the group
3. Prefer the most recently added phrasing when merging
4. Update the Corrections section in the persona SKILL.md - replace
   all the merged entries with the consolidated rule
5. Notify the user:

```
The corrections list reached 50 entries. I consolidated {N} similar corrections into {M} rules.
No behaviour was lost - the rules are now more general.
```

---

## Important Constraints

- **Never edit Layer 0–5 base content directly** as a result of a correction. Corrections
  always go into the `## Corrections` section. The Corrections section overrides the base
  layers - it does not replace them. This preserves the original distillation intact and
  makes corrections auditable.
- The only exception: if the user explicitly says "update the base persona" or "this is
  wrong at the foundation level", then edit the relevant base layer directly and do not add
  a correction entry.
- Do not correct things the user didn't ask to correct. Process one correction at a time.

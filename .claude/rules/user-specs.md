# User Specs

`Users Directory/User Specs/` is where the team writes down, before Laufey
acts, anything that needs input first or is big: answers to Laufey's
questions, inputs for a deliverable, drafts to refine or review, plans, and
requirements to record. Laufey reads a spec with `/read-spec`, which routes
it to the right skill or agent.

- **Specs are the team's files.** Never edit or delete one unless asked.
  Laufey's output goes to `AI Directory/Generated Outputs/` (or the place
  `file-placement.md` says), and Laufey says which spec it was based on.
- **Laufey may create new spec files** in that folder when it needs input
  first: an inputs sheet with the questions pre-filled for the team to
  answer. Name it `<Topic> - Inputs.md`. Never overwrite an existing spec.
- **Only act on specs marked `status: ready`.** A `draft` spec is still
  being written; say so and stop.
- **Frontmatter** at the top of each spec says what it is (see
  `.claude/skills/read-spec/spec-template.md`). If it is missing, infer the
  type, state it in one line, and confirm before acting.
- A spec's `format` field counts as the answer to the "ask the format first"
  rule in `file-placement.md`.
- **Stay lean.** The team's Claude credits are limited. Read only the files
  a spec names, reuse `MemoryBank.md` instead of rereading transcripts, and
  don't start a subagent unless the work needs one.

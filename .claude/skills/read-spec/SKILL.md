---
name: read-spec
description: Read a spec the team wrote in Users Directory/User Specs/ (inputs for a deliverable, a draft, a plan, a requirement, an issue) and route it to the right skill or agent. Use when someone says a spec is ready, points to a file in User Specs, asks Laufey to "read the spec", or asks what specs are waiting.
argument-hint: "[spec file name] | (blank to list specs)"
---

# Read a spec and route it

Rules for the folder are in `.claude/rules/user-specs.md`. Follow them.

## 1. Find the spec

- With a file name, read that file in `Users Directory/User Specs/`.
- With no argument, list the specs there with their `type`, `for`, `owner`,
  and `status`, and ask which one to act on. Don't open them all.

## 2. Check it is ready

- Read the frontmatter (template: `spec-template.md` in this folder).
- `status: draft`: say it isn't marked ready and stop.
- No frontmatter: infer the type from the content, say in one line what you
  inferred, and wait for a yes.
- Check the assignment it names against `AI Directory/Assignments.md`. If it
  conflicts with what the professor asked for, say so before acting.

## 3. Route by type

| `type` | What it is | Send it to |
|---|---|---|
| `inputs` | Answers for a TOGAF deliverable | `/build-deliverable` |
| `draft` | A team draft | `goal: review` (default): `/analyze-document`, which uses the `deliverable-reviewer` agent. `goal: refine`: `/build-deliverable` in refine mode |
| `plan` | A plan or approach to stress-test or build | `/plan-work` |
| `requirement` | What the professor asked for or said | `/log-assignment` |
| `issue` | A problem, blocker, or disagreement | `/log-issue` |
| `summary` | A request to condense documents | `/summarize-document` |
| `guide` | A request for a study guide | `/make-study-guide` |

Tell the person in one line which route you chose and why, then run it
with the spec's path, `mode`, and `format` passed along.

## 4. If a job needs input first

When someone asks for a deliverable and no `inputs` spec exists, don't ask
the questions one by one in chat. Offer to create
`Users Directory/User Specs/<Topic> - Inputs.md` from `spec-template.md`,
with the questions for each section of the template pre-filled and
`status: draft`. The team answers in the file and sets `status: ready`.

## 5. After

- Never edit the spec. Say which spec the output is based on.
- If the spec answers an Open Question in `MemoryBank.md` or reveals a new
  decision, say so and offer `/log-session` when the work is done.

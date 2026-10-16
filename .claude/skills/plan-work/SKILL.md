---
name: plan-work
description: Turn a goal or assignment into a concrete plan with tasks, owners, dates, dependencies, and risks, or stress-test a plan the team proposes. Use when asked to plan, schedule, break down or divide work, make a timeline, decide "what should we do next", or when someone proposes an approach and asks what you think.
argument-hint: "[goal or assignment] | review: [their plan]"
---

# Plan work

There are two modes. If the person describes **their own** plan or
approach, use mode B. Otherwise use mode A.

## Mode A: make a plan

1. **Pin down the goal and deadline.** Look the assignment up in
   `AI Directory/Assignments.md`. If it isn't recorded, ask for the
   requirements and deadline, and offer `/log-assignment`.
2. **Check context.** Read the Key Decisions and Open Questions in
   `MemoryBank.md`, plus open issues in
   `Users Directory/Issues/CurrentIssues.md`. A plan that ignores a known
   blocker is a bad plan.
3. **Ask only what you can't infer.** Usually that's who is available,
   and any dates people can't work. Ask in one short message.
4. **Build the plan backwards from the deadline.**
   - Break the work into tasks that each fit in one sitting.
   - For each task give: owner (Em, Clark, or Aldrin, or "team"), due date,
     what it depends on, and what "done" looks like.
   - Propose a split of the work, but the team decides who does what.
   - Leave at least one day of buffer before the deadline.
   - Include a review step before submission (`/analyze-document` with
     the `deliverable-reviewer` subagent).
   - Mark the critical path, meaning the tasks that delay everything if
     they slip.
5. **List risks and assumptions**, and anything worth asking the
   professor or the CSA stakeholders before starting.

Present the tasks as a table:

| # | Task | Owner | Due | Depends on | Done when |
|---|---|---|---|---|---|

## Mode B: stress-test the team's plan

1. Restate their plan in 2–3 lines and confirm you understood it.
2. **What's strong** about it, briefly.
3. **Risks, gaps, and hidden assumptions**, each with why it matters. Hold
   it against the professor's recorded requirements and feedback.
4. **At least one real alternative**, with its trade-offs.
5. **Your recommendation**, and what would change your mind.

Don't just approve the first idea. If the plan really is good, say so,
and say what you checked.

## After

- Keep the plan in the chat unless asked for a file. If asked, ask the
  format (unless given) and save it as
  `AI Directory/Generated Outputs/YYYY-MM-DD - Plan - <Topic>.<ext>`.
- Once the team agrees on a plan or a choice, record it under Key
  Decisions in `MemoryBank.md`, with the date.

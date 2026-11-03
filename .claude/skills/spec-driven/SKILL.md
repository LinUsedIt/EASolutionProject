---
name: spec-driven
description: Spec Driven Approach for producing ADM documents and diagrams. Two modes the team picks from - A (brainstorm in chat, then generate) or B (brainstorm, generate an inputs worksheet, team fills it, review, then generate). Use when the team asks to start, plan, or generate any ADM phase output, or says "approach A", "approach B", or "spec driven".
argument-hint: "[A|B] [phase or topic]"
---

# Spec Driven Approach

Every ADM output is designed first, then generated. Ask the team which
approach they want unless they already said. Recommend **A** when the team
already knows the content and the task is small; recommend **B** when
inputs are missing, the output is large, or the team wants to learn by
filling in the inputs themselves.

Before either approach: read `AI Directory/Assignments.md`, `MemoryBank.md`,
and the matching template in `Course Files/TOGAF Templates/`. Keep it lean;
don't reread transcripts that `MemoryBank.md` already summarizes.

## Approach A: chat, design, generate

1. **Context and tasks.** The team gives them in chat.
2. **Brainstorm a design.** Propose which documents and diagrams are
   needed (one per template, only the necessary ones), what each contains,
   and where its content comes from. Ask your questions and raise concerns
   and risks. Keep questions batched and numbered.
3. **Generate.** Once the team has answered and is satisfied with the
   design, run `/build-deliverable` for each document. Drafts go to
   `AI Directory/Generated Outputs/`.
4. Ask for approval. On approval, run `/publish-output`.

## Approach B: worksheet driven

1. **Context and tasks.** The team gives them in chat.
2. **Brainstorm a design.** Recommend which documents need to be created,
   and ask questions and raise concerns.
3. **Generate the worksheet** once those are answered. Create
   `Users Directory/User Specs/Worksheets/<Phase> - <Topic> - Worksheet.<ext>`
   (ask the format once if not given; Markdown by default). Never overwrite
   an existing worksheet; use ` (v2)`. Use the frontmatter from
   `.claude/skills/read-spec/spec-template.md` with `type: inputs` and
   `status: draft`. The worksheet must have:
   - **What Laufey already knows**, pre-filled per section, with the source
     file and date (`sources-and-citations.md`). The team confirms or
     corrects it.
   - **For each document:** a plain explanation of what it contains and why
     TOGAF asks for it (cited), then each section with (a) what to write,
     (b) how that section feeds the rest of the architecture, and (c) the
     answer area. "Unknown" is a valid answer.
   - A short list of **open questions** for the team.
4. **Team fills it** and saves it in that folder, then sets `status: ready`.
   Laufey reviews it (`/read-spec`) and asks any remaining questions, listing
   gaps and conflicts with the evidence. Don't edit the worksheet.
5. **Generate** the documents from the worksheet with `/build-deliverable`.
   Anything still unknown is marked `[TO CONFIRM: ...]`, never invented.
6. Ask for approval. On approval, run `/publish-output`.

## Either approach

- Say in one line which approach is running and what step you are on.
- Don't generate before the team confirms the design (A) or the worksheet
  is `status: ready` and questions are answered (B).
- After the set is done, run `/analyze-document` with `deliverable-reviewer`
  once across all documents, before asking for approval.

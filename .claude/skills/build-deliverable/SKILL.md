---
name: build-deliverable
description: Turn the team's inputs spec into one TOGAF deliverable document, using the official template in Course Files/TOGAF Templates/, and (in coach mode) explain why each section exists and what was changed. Use when a spec of type inputs is ready, or when asked to generate, write, or refine a Phase A to D deliverable such as the Architecture Vision or Capability Assessment.
argument-hint: "[spec file name] [coach|full] [refine]"
---

# Build a TOGAF deliverable from a spec

Usually reached through `/read-spec`. One run builds one deliverable. For
several, run once per document, and review the set together at the end.

## 1. Gather, and keep it lean

- Read the spec, the matching template, and the assignment in
  `AI Directory/Assignments.md`. Use `MemoryBank.md` and the transcripts
  the spec points to; don't reread other files.
- Get the template's section list from the `.docx` using the fallbacks in
  `.claude/rules/file-formats.md` (no pandoc on some laptops: `python-docx`,
  or unzip `word/document.xml`). Phases C and D have no fill-in template,
  only the recommended artifacts list in
  `Architecture Deliverables Phases C and D.docx`. Build those from the
  artifact names the spec chooses.

## 2. Gap check before writing

Map every template section to where its content comes from:

- **In the spec.**
- **In the repo** (memory, transcripts, notes). Cite the file and date,
  as `sources-and-citations.md` says.
- **Missing.** Never invent it. Put `[TO CONFIRM: <what is needed>]` in
  that spot.

If a missing item blocks several sections, stop and list the gaps, and offer
a new `<Topic> - Inputs.md` spec. Otherwise continue and report the gaps at
the end.

## 3. Write it

- Keep the template's headings and numbering. Fill the tracking and version
  tables. Remove instructional boilerplate that no longer applies.
- Refine the team's wording: concise, business language ("speak business,
  not tech"), consistent terms. Don't change a fact or a decision. If an
  input conflicts with the evidence (for example the registrar's speed in
  the SSE interview versus other interviews), flag it instead of choosing.
- Don't claim a TOGAF fact without a source. Cite book and page for TOGAF
  claims; use the `togaf-researcher` agent only when a claim needs a
  citation and the study guides don't cover it.
- Save per `.claude/rules/file-placement.md`:
  `AI Directory/Generated Outputs/YYYY-MM-DD - Phase <X> - <Template>.<ext>`
  with the spec's `format` (ask once if blank). Never overwrite; use `(v2)`.
- Reopen the file and check the text and tables came out right.
- `refine` mode: the input is the team's own draft. Save a revised version
  in `Generated Outputs`, say which file it is based on, and never touch
  the original.

## 4. Tell the person what happened

- **coach** mode (default): a short note per section: why TOGAF asks for it
  (one or two lines, with source), what the inputs said, what you changed
  and why, and what is still `[TO CONFIRM]`. The person is learning TOGAF by
  applying it, so teach through their own content.
- **full** mode: just the file path, the gaps, and the conflicts.
- Either way, list the choices you made so they can redirect you.

## 5. After

- When the set is done and before submission, run `/analyze-document` with
  the `deliverable-reviewer` agent once over all of them.
- Offer `/log-session`, and `/log-issue` for any gaps or conflicts the team
  should track.

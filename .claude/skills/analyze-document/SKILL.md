---
name: analyze-document
description: Critically assess a document (a team draft, an interview transcript, the professor's instructions, or a reading) against TOGAF and the professor's requirements, or check several documents for consistency with each other. Use when asked to review, assess, critique, check, evaluate, grade, or find gaps, weaknesses, or contradictions.
argument-hint: "[file(s)] [what to focus on]"
---

# Analyze a document

This skill judges a document. If the person only wants to know what a
document says, use `/summarize-document` instead.

## 1. Pin down what you're analyzing and against what

- Which file or files? If they're vague ("the proposal"), list the likely
  candidates and ask which one.
- What's the yardstick? Usually an assignment in
  `AI Directory/Assignments.md`. If it's not obvious which one applies,
  ask. If the professor's requirements for it aren't recorded yet, say so
  and offer `/log-assignment` first.
- Is there a focus? For example "just the RACI", "is it TOGAF-correct",
  or "does it answer Sir's WHY feedback". If none is given, do a full pass.

## 2. Read everything relevant

- Read the target document(s) in full. Don't skim.
- Read the professor's recorded requirements and feedback for that
  assignment.
- For facts about the enterprise, use the interview transcripts and
  notes in `Users Directory/Course Assignments/`.
- For TOGAF correctness, ask the `togaf-researcher` subagent for cited
  excerpts. Don't rely on memory.

## 3. Choose who does the judging

- **The team's graded work, or anything you (Laufey) drafted:** hand the
  review to the `deliverable-reviewer` subagent. Give it the file paths,
  the assignment, and the focus. It hasn't seen how the work was
  produced, so you aren't grading your own work. Then check its findings:
  drop anything without a concrete location and reason, and add anything
  important it missed.
- **Readings, transcripts, the professor's instructions:** analyze them
  yourself. Cover what the document establishes, what it leaves unclear,
  and what it means for the team's work.

## 4. Report

Use this structure:

1. **Verdict.** 2–3 plain sentences. How good is it, and what's the
   single most important thing to fix?
2. **Findings** as a table:

   | # | Severity | File and location | Issue | Why it matters (cited) | Suggested fix |
   |---|---|---|---|---|---|

   - **Critical:** fails a professor requirement, contradicts itself on
     scope, or gets a TOGAF concept wrong.
   - **Moderate:** a real gap or inconsistency a grader would likely notice.
   - **Minor:** polish that makes the work clearer or more convincing.
3. **What's working.** A few short bullets on what to keep, so revisions
   don't break it.
4. **Open questions.** Things only the team, the professor, or the CSA
   stakeholders can answer.

**Cross-document mode:** when checking several documents against each
other, the location column names both places. Look especially for
contradictions in scope, numbers, names, terminology, and commitments.

## 5. Follow up

- Offer to log Critical and Moderate findings with `/log-issue`. Don't
  log them without a yes.
- Don't rewrite the document unless asked. Fixing it is a separate
  request, and the revised version goes in `Generated Outputs`.
- If the person wants the analysis saved, ask the format first (unless
  given) and save it as
  `AI Directory/Generated Outputs/YYYY-MM-DD - Analysis - <Document>.<ext>`.

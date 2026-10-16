---
name: summarize-document
description: Write a faithful, condensed summary of one or more documents, such as readings, interview transcripts, notes, drafts, or the professor's instructions. Use when asked to summarize, recap, give the gist or key points, or "what does this say".
argument-hint: "[file(s)] [short | medium | long]"
---

# Summarize a document

A summary reports what the document says, without judging it. If the
person wants an assessment, use `/analyze-document`. If they want study
material for a TOGAF chapter, suggest `/make-study-guide`.

## Length

Use what the person asked for. Otherwise default to **medium**.

- **Short:** 3–5 bullets.
- **Medium:** about one page: key points plus important details.
- **Long:** section by section, following the document's own structure.

Don't ask about length. Just mention at the end that a shorter or longer
version is available.

## Structure

1. **What it is:** one line with title, author or speaker, date, and type
   of document.
2. **Key points:** the main ideas, in the document's own order of
   importance.
3. **Important details:** numbers, names, dates, decisions, deadlines,
   and commitments, copied exactly.
4. **Key quotes:** short verbatim quotes for the claims that matter most,
   with page or timestamp.
5. **What this means for us** (optional, only when relevant): a clearly
   separated section labeled as Laufey's take, connecting the document to
   the team's current assignment in `AI Directory/Assignments.md`.

## Faithfulness

- Don't add anything that isn't in the source. Keep your opinions out of
  sections 1–4.
- **Transcripts:** keep speakers distinct, so it's clear who said what
  (for example Ms. Nina versus Ms. Kelai).
- **The team's notes:** keep their uncertainty. If the notes say "(???)"
  or "IDK what I wrote here", flag it as unclear instead of guessing.
- **TOGAF readings:** cite pages, and keep what the Standard says separate
  from the author's opinion.
- When several documents disagree, say so instead of blending them.

## Output

Give the summary in the chat by default. If the person wants a file, ask
the format (unless given) and save it as
`AI Directory/Generated Outputs/YYYY-MM-DD - Summary - <Document>.<ext>`.

---
name: make-study-guide
description: Create a study guide for a chapter of Mastering the TOGAF Standard, or for a topic or section of the other course Readings, saved in Course Files/Study Guides. Use when asked for a study guide, reviewer, study notes, or exam prep on a chapter or TOGAF topic.
argument-hint: "[chapter number or topic]"
---

# Make a study guide

## 1. Identify the source

- **A chapter number** means Jager's *Mastering the TOGAF Standard*. Use
  that chapter's PDF in
  `Course Files/Readings/Mastering the TOGAF Standard - Segmented/`.
- **A topic** ("Phase B", "building blocks"): find where it's covered.
  Use the `togaf-researcher` subagent if you're not sure which book or
  chapter. Then confirm the source and scope with the person.

## 2. Check what already exists

Look in `Course Files/Study Guides/` first. If a guide for that chapter
already exists, say so and ask whether they want a new version ` (v2)` or
something else, such as practice questions only.

## 3. Ask before generating

Unless the person already said, ask in **one** message:

- the format: Markdown, Word, or PDF (the existing guides are PDFs), and
- the target folder and file name you plan to use, so they can confirm.

## 4. Read the source properly

- Read the whole chapter, page range by page range. Don't summarize from
  the table of contents.
- Note page numbers as you go. Every point in the guide needs one.
- Note where Jager gives his own opinion as opposed to what the Standard
  says.
- For cross-references to the TOGAF Standard itself, ask
  `togaf-researcher` for cited excerpts.

## 5. Write it

Follow [template.md](template.md) exactly, so all guides match. Keep the
plain, clear register of the existing guides. Laufey's playful tone
doesn't belong in a study guide.

## 6. Check it

Before saving, confirm that:

- every numbered section of the chapter appears in the Detailed Section
  Breakdown,
- every bullet and every self-check answer has a page reference,
- the self-check answers are actually right (re-check them against the
  pages), and
- author opinions are labeled.

## 7. Save it in the Study Guides folder, not Generated Outputs

`Course Files/Study Guides/<range folder>/Chapter N - <Chapter Title> - Study Guide.<ext>`

- Range folders: `TOGAF Ch1-7`, `TOGAF Ch8-9`, `TOGAF Ch10-12`. For any
  other chapter, ask which folder to use.
- Use plain ASCII in the file name.
- If it's Word or PDF, reopen it and check it renders correctly.
- There's also a compiled guide,
  `Mastering the TOGAF Standard - Compiled Study Guide (Ch 1-12).pdf`. Ask
  whether it should be updated too. Don't change it on your own.

Then run `/log-session` or note the new guide for the next log.

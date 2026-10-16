---
name: log-session
description: Record the current work session in AI Directory/SessionLog.md and bring MemoryBank.md up to date. Use at the end of a session, after a substantial piece of work, when someone says they're done or leaving, or when asked to log, record, or save what happened.
---

# Log the session

## 1. Gather the facts

- **Date:** today's date, written as YYYY-MM-DD.
- **Participants:** which team member(s) plus Laufey. Ask if you don't know.
- **What happened:** what was discussed, decided, and produced, including
  the paths of files created or changed.

## 2. Write the entry

Use the exact format shown at the top of `AI Directory/SessionLog.md`, with
every field filled in. The summary must make sense to a teammate who wasn't
there and can't see the conversation: name the documents, the reasoning,
and the conclusions. Write "None" for an empty field. Don't drop it.

Insert the entry **at the top** of the entries in `SessionLog.md` (newest
first). Two sessions on the same day get two separate entries.

**Backfilled entries:** if you're recording work that happened in an
earlier session you weren't part of (reconstructed from git history or
files), add `(reconstructed)` to the title, and say in the summary what it
was reconstructed from.

## 3. Update MemoryBank.md

- **Snapshot:** overwrite anything now out of date (current focus, what's
  due next). Don't append duplicates.
- **Key Decisions:** append decisions made this session, as
  `**YYYY-MM-DD:** decision. Reason: ...`.
- **Open Questions:** add new ones. Move answered ones to Key Decisions.

## 4. Check nothing was missed

- Professor's requirements or feedback mentioned this session should be in
  `Assignments.md` (use `/log-assignment`).
- Issues raised this session should be in the tracker (use `/log-issue`).

## 5. Confirm

Tell the person in 2–3 lines what you logged and what changed in the
memory bank.

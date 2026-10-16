---
name: log-issue
description: Add, update, resolve, or list issues in the tracker, keeping Users Directory/Issues/CurrentIssues.md and CurrentIssuesList.csv in sync. Use when a blocker, risk, disagreement, problem, or review finding needs tracking, or when asked to log, close, update, or list issues.
argument-hint: "[add | update ISS-00X | resolve ISS-00X | list]"
---

# Log an issue

Both files live in `Users Directory/Issues/`. Read **both** before
changing either.

## Add

1. **Check for duplicates.** If the problem is already open, update that
   entry instead.
2. **Pick the next ID:** the highest ID found in *either* file, plus one,
   as `ISS-` followed by three digits. Never reuse an ID.
3. **Add to `CurrentIssues.md`** under **Open Issues**, in the exact
   format shown at the top of that file. Remove the `_(none yet)_`
   placeholder if it's there.
4. **Add the matching row to `CurrentIssuesList.csv`**, with columns
   `ID,Issue,Date Recorded,Possible Solutions,Resolved,Date Resolved`:
   - Put every text field in double quotes, and double any quote marks
     inside it (`"He said ""no"""`).
   - Join multiple possible solutions with ` | `.
   - `Resolved` is `No` or `Yes`.
   - `Date Resolved` is left empty while open. In the .md file it's `—`.
   - Keep the CSV in plain characters (no em dashes or curly quotes), so
     it opens cleanly in Excel.

## Update

Change the same entry in both files: add a solution, clarify the
description, and so on. Don't change the ID or the date recorded.

## Resolve

Only resolve an issue when a team member confirms it's fixed. A fix you
drafted doesn't count until they accept it.

- In `CurrentIssues.md`, set **Resolved: Yes** and the date, then move the
  entry from **Open Issues** to **Resolved Issues**. If it's the first
  resolved one, remove the placeholder.
- In the CSV, set `Resolved` to `Yes` and fill in `Date Resolved`.

## List

Read `CurrentIssues.md` and give a short list of the open issues (ID,
title, date recorded), oldest first.

## Verify

After any change, check that both files contain exactly the same set of
IDs, with the same resolved status. If they don't, fix the mismatch and
tell the person.

# Issue logging

Any issue that comes up (a blocker, a disagreement, a technical problem, a
gap found in a review, anything worth tracking) gets logged in **both**
files in `Users Directory/Issues/`:

- `CurrentIssues.md`, which is human-readable
- `CurrentIssuesList.csv`, which is the same data as a table

Use `/log-issue` to add, update, or resolve issues. It keeps both files in
sync.

- The two files must always match, with the same IDs.
- IDs are sequential (`ISS-001`, `ISS-002`, ...) and never reused, even
  after an issue is closed.
- Every entry records: what the issue is, the date recorded, possible
  solutions, whether it's resolved, and the date resolved.
- Follow the exact layout shown at the top of `CurrentIssues.md`.
- Only mark an issue resolved when a team member confirms it, not when you
  think a fix you drafted would solve it.
- Don't log the same problem twice. If it's already open, add to the
  existing entry.

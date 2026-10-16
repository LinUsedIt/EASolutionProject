# Memory

The team's shared memory lives in three files in `AI Directory/`. They're
in git, so every team member's Laufey sees the same history.

| File | What it holds | Loaded automatically? |
|---|---|---|
| `MemoryBank.md` | Project snapshot, key decisions, open questions | Yes |
| `Assignments.md` | Everything the professor has asked for | Yes |
| `SessionLog.md` | One entry per session, newest first | No, read it when needed |

## Check memory first

Before answering anything about the project's history, past discussions,
plans, or decisions, check `MemoryBank.md`, and then `SessionLog.md` if you
need detail. Don't guess from partial context or assume nothing was
decided. If memory and the current conversation disagree, say so
explicitly instead of silently picking one.

## Log every session

Run `/log-session`:

- after any substantial piece of work,
- whenever the person signals they're wrapping up ("that's all", "thanks,
  bye", "I'll continue later"), and
- at the start of a session, if you can see from git or the files that
  work happened since the last log entry. In that case, offer to backfill
  it and mark the entry as reconstructed.

Follow the entry format in `SessionLog.md` exactly. Don't skip fields.

## Keep the snapshot current

`MemoryBank.md` is a current-state snapshot, not a diary. Overwrite
outdated facts in the Snapshot section in place. Append to Key Decisions
and Open Questions. When an open question gets answered, move it to Key
Decisions with the date.

## Claude Code's own auto memory

Claude Code may also keep private notes on each person's computer. Those
aren't shared with the rest of the team. Anything that matters to the
project goes in these three files, and if the two ever disagree, these
files win.

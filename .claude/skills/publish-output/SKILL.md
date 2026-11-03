---
name: publish-output
description: Save an approved document or diagram into OSM Architecture/ with the standard name and version, and move the superseded version to Archive. Use when the team says an output is approved, final, or ready for the repo.
argument-hint: "[file in Generated Outputs] [version]"
---

# Publish an approved output to OSM Architecture

Rules: `.claude/rules/osm-architecture.md`. Only run this after a team member
explicitly says the output is approved. Never publish on your own judgment.

1. **Confirm** the source file, the phase, and the version (`v0.x` draft
   submitted for review, `v1.0` first approved baseline, `v1.1` small
   revision, `v2.0` major rework). Ask once if unclear.
2. **Name it** `<Title> - v<X.Y>.<ext>`: no date, no assignment identifier
   (strip `YYYY-MM-DD - A<n> - Phase <X> -` from the draft name). ASCII only.
3. **Copy** it into the phase folder (diagrams into `Diagrams/`); never move
   the original. If an earlier version exists, move that file to the phase's
   `Archive/` folder.
4. **If it belongs to a repository component** (metamodel, requirements,
   standards, governance, and so on), also place it in
   `OSM Architecture/Architecture Repository/<component>/`.
5. **Add nothing else** to `OSM Architecture/`: no README or index. Remove a
   folder's `.gitkeep` once it has real files.
6. Reopen the file to check it opens. Report the new path in one line and
   offer `/log-session`.

# OSM Architecture (the submission folder)

`OSM Architecture/` sits beside `AI Directory/`, `Course Files/`, and
`Users Directory/`. The repo is shared with Sir Pira on GitHub, and this
folder is what he reviews: **approved outputs only**, organized by ADM
phase plus the TOGAF Architecture Repository components (Jager 2025,
Ch. 7, pp. 129-136).

## What goes in

- Drafts go to `AI Directory/Generated Outputs/`. They move into
  `OSM Architecture/` only when a team member says they are approved, using
  `/publish-output`. Never publish unapproved work.
- **No README, index, notes, or other helper files** inside
  `OSM Architecture/`. Sir sees only deliverables. Empty folders hold a
  `.gitkeep` so git keeps them. No drafts, transcripts, or internal notes.
- Don't edit approved files in place. A change is a new version; the old
  one moves to the phase's `Archive/` folder.

## Structure

- Phase folders: `Preliminary`, `Phase A - Architecture Vision`,
  `Phase B - Business Architecture`, `Phase C - Information Systems
  Architectures`, `Phase D - Technology Architecture`, `Phase E` to `Phase H`,
  `Requirements Management`. Diagrams go in a `Diagrams/` subfolder.
- `Architecture Repository/` has one subfolder per component: Architecture
  Metamodel, Architecture Landscape (Strategic, Segment, Capability),
  Solutions Landscape, Architecture Requirements Repository, Reference
  Library, Standards Library, Governance Repository, Architecture Capability.
  Phase folders hold the deliverables; these hold reusable and governing
  assets.

## Naming

- **Drafts** (in `Generated Outputs/`) carry the assignment identifier:
  `YYYY-MM-DD - A<n> - Phase <X> - <Title> (v2).ext`.
- **In `OSM Architecture/`** drop the date and the assignment identifier:
  `<Title> - v<major>.<minor>.<ext>`, for example
  `Architecture Vision - v0.1.docx`. Plain ASCII.
- **Versions:** `v0.x` submitted draft, `v1.0` first approved baseline,
  `v1.1` small revision, `v2.0` major rework.

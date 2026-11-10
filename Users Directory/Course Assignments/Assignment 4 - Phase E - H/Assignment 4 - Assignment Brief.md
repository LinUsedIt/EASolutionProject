# Assignment 4: Assignment Brief (Phases E to H)

Prepared 2026-11-10 by Laufey, for Em, Clark, and Aldrin.
Companion files in this folder: `Assignment 4 - Deliverables List.md` and
`Assignment 4 - OSM Meeting Questions.md`.

## 1. At a glance

| | |
|---|---|
| **Task** | Finish the remaining ADM phases: Phase E, F, G, H (plus Requirements Management) |
| **Enterprise** | Mentoring Unit (Office of Student Mentoring), CSA, UA&P |
| **Deadline** | **2026-11-27 (Friday)**, relayed by Em on 2026-11-10; not yet confirmed as Sir Pira's date |
| **Submission** | Approved outputs in `OSM Architecture/`, published to the G7-Repository on GitHub |
| **Also required** | The TOGAF Enterprise Architecture Checklist, kept in the G7-Repository and updated whenever phases change. **The team writes it, not Laufey** (Sir Pira, relayed 2026-11-10) |
| **Days left** | 17 calendar days from 2026-11-10 |

## 2. What is confirmed and what is not

**Confirmed (relayed by Em):** the task, the 2026-11-27 deadline, the GitHub
submission, and the Checklist requirement.

**Not confirmed (do not treat as Sir's rules yet):**
- Whether all templates in Phases E to H are expected, or only the necessary
  ones, and whether it is one document per template. (For Assignment 3 the
  team chose "only what is necessary"; Em's reading, not confirmed.)
- Whether Requirements Management and the Preliminary Phase count.
- Where the Checklist goes in the repo, its format, and whether there is a
  template.
- Whether 2026-11-27 is Sir's own date.

Ask Sir about these first; the answers change the amount of work.

## 3. Objective

Take the architecture from Phases A to D (what the unit is, what is wrong,
what it should become) and finish the **plan to get there and the
governance around it**:

- **Phase E:** what to do and in what order.
- **Phase F:** how to move safely, and who oversees it.
- **Phase G:** how to check what is built matches the architecture.
- **Phase H:** how to handle changes after launch.
- **Requirements Management:** keep the requirements current throughout.

Sir Pira's earlier feedback still applies: start from the business's **WHY**,
not the HOW. The work packages must visibly serve the unit's purpose (a
uniform, centralized mentoring program) and the 3-sessions catalyst.

## 4. Starting point (what already exists)

| Item | Where | State |
|---|---|---|
| Phase A documents (Vision, Statement of Architecture Work, Capability Assessment) | `OSM Architecture/Phase A - Architecture Vision/` | v0.1, submitted |
| Phase B documents (Requirements Specification, Roadmap) | `OSM Architecture/Phase B - Business Architecture/` | v0.1, submitted |
| Phase C and D combined document | `OSM Architecture/Phase C...` and `Phase D...` | v0.1, submitted |
| Preliminary work in the Roadmap | Roadmap sections 3.1 (work packages WP1 to WP4), 3.2, 3.5 | Marked "to be confirmed in Phase E" |
| Open issues | `Users Directory/Issues/CurrentIssues.md` | ISS-009 to ISS-012 touch these documents; ISS-010 (approval chain) matters for Phase F |
| Open "who manages the tools" conflict | `MemoryBank.md` | Unresolved; matters for Phase F |

## 5. Deliverables

Proposed (full reasoning in `Assignment 4 - Deliverables List.md`). Names in
`OSM Architecture/` follow `<Title> - v<major>.<minor>`.

| # | Deliverable | Phase | Status of decision | Needs from the OSM |
|---|---|---|---|---|
| E1 | Implementation and Migration Plan | E (finalized in F) | Include | Priorities, timing, dependencies, resources |
| E2 | Architecture Roadmap (new version) | E | Include | Same as E1 |
| E3 | Project Context Diagram | E | Include | Who is involved in each work package |
| E4 | Benefits Diagram | E | Include | What success looks like |
| F1 | Implementation Governance Model | F | Include | Ownership, approval, review rhythm |
| F2 | Architecture Contract | F | **Team decides** | Who the implementer is |
| F3 | Architecture Building Blocks | F | **Team decides** | None (from Phases B to D) |
| G1 | Compliance Assessment | G | Include | What "working" means, who checks |
| G2 | Solution Building Blocks | G | **Team decides** | Any platform choice |
| H1 | Change Request (worked example) | H | Include | How changes are handled today |
| H2 | Requirements Impact Assessment (worked example) | H | Include | Same as H1 |
| R1 | Architecture Requirements Specification (new version) | RM | Include | A check that requirements still hold |
| X1 | TOGAF Enterprise Architecture Checklist | all | Team writes | None |

Sources: the templates are in `Course Files/TOGAF Templates/`; the Phase E
diagrams are from Jager 2025, Ch. 7, p. 163.

## 6. What we need from the OSM

One meeting (30 to 45 minutes) with Ms. Nina and Ms. Kelai, ideally with a
word from the sponsor (CSA Executive Director) and the IT Office. The
plain-language reasons and 21 sample questions are in
`Assignment 4 - OSM Meeting Questions.md`.

**Essential questions** (if time or access is limited, ask these 8): 1, 2, 4,
7, 9, 12, 13, 16.

## 7. How we work (Spec Driven Approach)

Use `/spec-driven`. **Recommended: Approach B** for most documents, because
E, F, G, and H have many unknowns that the OSM meeting will answer.

1. Laufey designs the set and asks questions.
2. Laufey generates one worksheet per phase in `Users Directory/User Specs/Worksheets/`, pre-filled with
   what we know and an explanation of each section.
3. The team fills the worksheets (after the OSM meeting) and sets `status: ready`.
4. Laufey reviews and asks remaining questions, then generates the documents.
5. The team approves; `/publish-output` places them in `OSM Architecture/`.

For small, well-known items (for example H1 and H2 worked examples),
Approach A (chat, then generate) is fine.

Draft names: `YYYY-MM-DD - A4 - Phase <X> - <Title> (v2).ext`.

## 8. Rules that apply

- Use TOGAF content **only** from the three course Readings, and cite book and
  page. Interview notes are evidence about the unit, not TOGAF sources.
- Plain ASCII file names. No Claude mentions in `OSM Architecture/`.
- Approved outputs only in `OSM Architecture/`. A new version replaces the
  old, which moves to `Archive/`.
- Unknown facts are marked `[TO CONFIRM]`, never invented.
- Publish with `git subtree push --prefix="OSM Architecture" sir main` after
  approval. Do not edit files in the G7-Repository directly.
- The Checklist is written by the team. Laufey does not draft it.

## 9. Proposed schedule

| Dates | What | Notes |
|---|---|---|
| 2026-11-10 to 11-12 | Ask Sir the open questions (section 2). Decide F2, F3, G2. Request the OSM meeting. Agree who owns which phase. | Em leads the message to Sir |
| 2026-11-12 to 11-13 | Laufey generates the worksheets (Approach B). Team starts what it can fill without the OSM. | |
| 2026-11-16 to 11-18 | **OSM meeting**, or send the 8 essential questions in writing | Target; adjust to their calendar |
| 2026-11-17 to 11-20 | Team completes worksheets with the answers. Laufey reviews and asks follow-ups. | |
| 2026-11-20 (Fri) | Laufey generates all drafts (E to H, plus Roadmap and ARS updates) | |
| 2026-11-23 to 11-24 | Team review. Independent review with `deliverable-reviewer`. Fix findings. Update the Checklist. | |
| 2026-11-25 | Team approves. Publish to `OSM Architecture/` and push to the G7-Repository. | |
| 2026-11-26 | Buffer | |
| **2026-11-27** | **Deadline** | |

Owners: no fixed roles. Suggested starting point, to be confirmed: Em takes
Phase E, Aldrin takes Phases F and G, Clark takes Phase H and Requirements
Management, mirroring the Assignment 3 split. The Checklist is shared.

## 10. Risks and watch-outs

| Risk | Why it matters | Response |
|---|---|---|
| The OSM meeting slips | Phases E to H depend on their answers | Book it early; send the essential questions in writing as a fallback |
| Invented content in E to H | These phases are mostly decisions, so it is easy to guess | Mark `[TO CONFIRM]`; label assumptions |
| Scope creep into implementation | Phase G and H are about governance, not building the platform | Keep worked examples small |
| Earlier documents conflict with new ones | ISS-009 to ISS-012 are still open | Fix in the next versions; log in the Checklist |
| Weekly Claude credits are limited | Many documents in a short time | Batch requests; use Approach B to avoid back-and-forth |
| Deadline is unconfirmed | Planning may be wrong | Confirm with Sir this week |
| Checklist forgotten again | Sir already flagged it | Add a "Checklist updated?" step before every publish |

## 11. Definition of done

- Every agreed deliverable exists in `OSM Architecture/` with a version number.
- All new content has no unresolved `[TO CONFIRM]` that the team has not
  consciously accepted.
- Earlier documents are updated where Phases E to H changed them.
- The Checklist is current and in the G7-Repository.
- The `deliverable-reviewer` has reviewed the whole set.
- G7-Repository shows the latest push, checked on GitHub.
- `Assignments.md`, `MemoryBank.md`, and the session log are updated.

## 12. Open questions

See section 2, plus:
- Which of F2, F3, and G2 does the team want?
- Can the sponsor and the IT Office attend or answer in writing?
- Should the mentors be consulted before the Phase G measures are final?

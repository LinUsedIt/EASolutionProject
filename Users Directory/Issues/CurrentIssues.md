# Current Issues — EASolutionProject

Tracks issues that come up over the course of the project — blockers,
disagreements, technical problems, anything worth remembering. Every issue
logged here must also appear as a row in `CurrentIssuesList.csv`, using the
same ID, so the two stay in sync.

## Entry Format

Each issue uses this format:

```
### [ISS-00X] — [Short title]

- **Issue:** what the issue is, in enough detail that someone unfamiliar
  with the moment understands the problem.
- **Date Recorded:** YYYY-MM-DD
- **Possible Solutions:**
  - option 1
  - option 2
- **Resolved:** Yes / No
- **Date Resolved:** YYYY-MM-DD, or "—" if still open
```

IDs are sequential (`ISS-001`, `ISS-002`, ...) and never reused, even if an
issue is later closed.

## Open Issues

### [ISS-001] — Scope contradiction on pairing and mentor-change processes

- **Issue:** Deliverable 1 excludes "the exact mentor-mentee pairing process... and mentor change approval" from its Functional boundary and lists pairing as Out of Scope. Deliverable 2 still commits to Business Process Diagrams for Pairing and Change of Mentor in Phase B, and its Value Stream runs through pairing and mentor confirmation. The documents disagree on whether these processes are in scope. Severity: Critical. This should be settled before any Phase A-E work, since it decides what Deliverable 2 may model. Logged from `AI Directory/Generated Outputs/Issues Log - First Draft Review.md` (finding #1).
- **Date Recorded:** 2026-09-15
- **Possible Solutions:**
  - Redraw the boundary: the unit's own part (receiving pairings, assessing and relaying change requests) is in scope; the schools' internal matching criteria and decisions are out of scope
  - Or drop the Pairing/Change of Mentor process diagrams from the Phase B commitments
  - Note: mentor-change requests are now the unit's biggest problem (2026-09-28 interview), which argues for keeping the unit's side in scope
  - A fix was drafted in Laufey's `Assignment 1 - Compiled Enterprise Proposal (Revised).docx` (see `Assignment 1 - Revision Notes.docx`), but the team never adopted it
- **Resolved:** No
- **Date Resolved:** —

### [ISS-002] — Business Catalyst omits the logging shift from mentor to student

- **Issue:** The most-cited business driver, that session-logging responsibility moved from mentor to student, appears in the Executive Summary, Deliverable 2 (Assumption entity), and Deliverable 3 (Business Goals, Change Driver), but not in Deliverable 1's own Business Catalyst paragraph, which covers only the 3-session quota and the enrollment consequence. Severity: Moderate. Logged from `AI Directory/Generated Outputs/Issues Log - First Draft Review.md` (finding #2).
- **Date Recorded:** 2026-09-15
- **Possible Solutions:**
  - Add a sentence on the logging-responsibility transfer to Deliverable 1's Business Catalyst section
  - A fix was drafted in Laufey's `Assignment 1 - Compiled Enterprise Proposal (Revised).docx` (see `Assignment 1 - Revision Notes.docx`), but the team never adopted it
- **Resolved:** No
- **Date Resolved:** —

### [ISS-003] — RACI roles can't be traced to real names

- **Issue:** Deliverable 1's RACI uses generic roles ("Student A (Organizational Architect)", "Student B (Framework and Metamodel Architect)"), while Deliverable 3's RFA "Prepared by" line uses real names (Deejay Clark Datu and Emmanual Velasco, sic). Nothing maps one to the other. Severity: Minor. Logged from `AI Directory/Generated Outputs/Issues Log - First Draft Review.md` (finding #3).
- **Date Recorded:** 2026-09-15
- **Possible Solutions:**
  - Use real names consistently (the team no longer has fixed roles, and Aldrin has joined)
  - Or add a one-line mapping of roles to names
  - A fix was drafted in Laufey's `Assignment 1 - Compiled Enterprise Proposal (Revised).docx` (see `Assignment 1 - Revision Notes.docx`), but the team never adopted it
- **Resolved:** No
- **Date Resolved:** —

### [ISS-004] — External mentors' route into approval is unexplained

- **Issue:** Deliverable 1 says mentor approval comes only from "the list of professors provided by each of the university's schools". Deliverables 2 and 3 refer to External Mentor Contracts and HR/FMR involvement, but no document explains how external (non-faculty) mentors enter the approval pipeline. Severity: Moderate. Logged from `AI Directory/Generated Outputs/Issues Log - First Draft Review.md` (finding #4).
- **Date Recorded:** 2026-09-15
- **Possible Solutions:**
  - Describe the external-mentor route using the 2026-09-28 interview: sourced by referral (alumni, speakers, former professors and employees), contracted through HR
  - Flag the confidential mentor approval scorecard as a known limit of the evidence
  - A fix was drafted in Laufey's `Assignment 1 - Compiled Enterprise Proposal (Revised).docx` (see `Assignment 1 - Revision Notes.docx`), but the team never adopted it
- **Resolved:** No
- **Date Resolved:** —

### [ISS-005] — Organizational boundary omits mentors and mentees

- **Issue:** The list of direct interfaces in Deliverable 1's Organizational boundary leaves out Mentors and Mentees, although the Stakeholder Map classifies both as Keep Informed and directly affected by any process or tool change. Severity: Minor. Logged from `AI Directory/Generated Outputs/Issues Log - First Draft Review.md` (finding #5).
- **Date Recorded:** 2026-09-15
- **Possible Solutions:**
  - Add mentors and mentees to the list of direct interfaces
  - A fix was drafted in Laufey's `Assignment 1 - Compiled Enterprise Proposal (Revised).docx` (see `Assignment 1 - Revision Notes.docx`), but the team never adopted it
- **Resolved:** No
- **Date Resolved:** —

### [ISS-006] — Principle 5 implications are thin

- **Issue:** Deliverable 3's Principle 5 ("Minimal Additional Burden on Staff") lists only two generic implications, versus three or four concrete ones for Principles 1, 2, and 4. It doesn't mention the single-school pilot the coordinators proposed (cited in Deliverable 2's Work Package justification). Severity: Minor. Logged from `AI Directory/Generated Outputs/Issues Log - First Draft Review.md` (finding #6).
- **Date Recorded:** 2026-09-15
- **Possible Solutions:**
  - Add concrete implications, such as piloting changes with one school (SSE, about 100 students) before wider rollout, and scoping training to the two coordinators
  - A fix was drafted in Laufey's `Assignment 1 - Compiled Enterprise Proposal (Revised).docx` (see `Assignment 1 - Revision Notes.docx`), but the team never adopted it
- **Resolved:** No
- **Date Resolved:** —

### [ISS-007] — Scale figures not carried into stakeholder and Measure reasoning

- **Issue:** Deliverable 3's RFA gives concrete scale figures (about 1,500-1,600 students, about 180 faculty mentors, 2 coordinators), but they never appear in Deliverable 1's stakeholder power/interest reasoning or Deliverable 2's Measure entity, where they would support feasibility and workload claims. Severity: Minor. Logged from `AI Directory/Generated Outputs/Issues Log - First Draft Review.md` (finding #7).
- **Date Recorded:** 2026-09-15
- **Possible Solutions:**
  - Reference the figures in the Stakeholder Map introduction and the Measure entity's justification
  - A fix was drafted in Laufey's `Assignment 1 - Compiled Enterprise Proposal (Revised).docx` (see `Assignment 1 - Revision Notes.docx`), but the team never adopted it
- **Resolved:** No
- **Date Resolved:** —

### [ISS-008] — Principle P2 implication is out of date

- **Issue:** One implication of Principle 2 (Data Consistency and Accuracy) in the A1/A2 Principles Catalog says the session-log database and the pairing database are isolated. Per the 2026-09-28 interview with OSM, the IT Office has since linked the session-log sheet to OSM's master database, so confirmed sessions update it automatically. What remains unlinked is OSM's database and the school coordinators' own pairing lists. Found while drafting Phases C and D (2026-10-30). Owner: Em.
- **Date Recorded:** 2026-10-30
- **Possible Solutions:**
  - Reword the implication: the session-log sheet now updates OSM's master database, but the coordinators' pairing lists are still separate
  - Or leave the A1 text as historical and rely on the Phase C baseline (Section 2.1 of the Phases C and D document), which states the corrected picture
- **Resolved:** No
- **Date Resolved:** —

### [ISS-009] — Non-compliance consequence: two or three semesters?

- **Issue:** The RFAW (A1) says two consecutive semesters of non-compliance affect enrollment. The Phase B ARS (Motivation) and the Phase B handoff brief say three, following Em's Notes 2. Clark confirmed on 2026-10-30 that two is correct. Phase A should use two.
- **Date Recorded:** 2026-10-30
- **Possible Solutions:**
  - Use two consecutive semesters in Phase A
  - Aldrin to correct the Phase B ARS (listed in the 2026-10-30 Phase B change list)
- **Resolved:** No
- **Date Resolved:** —

## Resolved Issues

_(none yet)_

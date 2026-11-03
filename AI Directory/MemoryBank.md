# Memory Bank: EASolutionProject

The team's shared, current-state memory. It loads automatically every
session. Laufey keeps it current with `/log-session`; rules are in
`.claude/rules/memory.md`. Full session history is in `SessionLog.md`, and
what the professor has asked for is in `Assignments.md`.

## Project Snapshot
_(Current-state facts. Overwrite in place as things change; don't append
duplicates.)_

- **Course:** IT Elective: Solution Architecture. The subject is
  Enterprise Architecture.
- **Professor:** Sir Pira.
- **Team:** Emmanuel Velasco ("Em"), Deejay Clark Datu ("Clark"), and
  Aldrin (joined around October 2026; surname not yet recorded). There are
  no fixed roles or deliverables. Work follows what the professor asks
  for (see `Assignments.md`).
- **Enterprise:** the Mentoring Unit (also called the Office of Student
  Mentoring), Center for Student Affairs (CSA), University of Asia and the
  Pacific (UA&P).
  - **Interviews:** 2026-09-11 with Ms. Nina and Ms. Kelai (Operations
    Coordinators), and a follow-up on 2026-09-28 with Ms. Nina. The
    transcripts and Em's notes are in the assignment folders. School
    Mentoring Coordinator interviews are complete for the SSE and SED
    schools (reported 2026-10-24). Both transcripts are in
    `Users Directory/Course Assignments/Assignment 3 - Phase A - D/Transcripts/`,
    but are mislabeled: `2026-10-16 interview.pdf` is Dr. Olmos (SSE), and
    `Mentoring Coordinator Interview - SSE.pdf` is Sir Lactao, School of
    Education (SED) (found 2026-10-29). Mentor interviews
    remain, using the coordinator question set modified for mentors.
    Coordinators are also mentors.
  - **Size:** 2 staff, one handling monitoring (Ms. Kelai) and one
    handling mentor training. About 1,500–1,600 undergraduates and about
    180 mentors. Sponsor: CSA Executive Director.
  - **Purpose (the WHY, from the 2026-09-28 interview):** the Mentoring
    Program is one of UA&P's hallmarks, supporting the integral
    (holistic) formation of students. The unit exists to keep the program
    uniform and centralized across schools.
  - **Catalyst:** from AY 2026-27, students must have at least 3 mentoring
    sessions per semester. Failing this for two consecutive semesters
    affects enrollment (per the RFAW; confirmed by Clark 2026-10-30, ISS-009). The requirement is non-negotiable. Participation
    became mandatory under the new university President.
  - **Current pain points:** a large number of mentor-change requests,
    handled by long email chains; dependence on the schools and the
    Registrar for pairings; uncertainty about whether students will log
    their sessions properly.
- **Current focus:** A3, Phases A-D (ADM), due 2026-10-30 (relayed by Em;
  not yet confirmed as Sir's date). Split (set 2026-10-27): Em does Phase A,
  Aldrin does Phase B, Clark does Phases C and D. Em gives inputs and
  Laufey refines and generates the documents, so Em learns and applies
  TOGAF himself. Submission is Friday 2026-10-30. All Phases A to D documents (version 0.1) are in
  `Users Directory/Course Assignments/Assignment 3 - Phase A - D/ADM Phases A - D/`,
  in `Phase A/`, `Phase B/`, `Phase C/`, and `Phase D/`. Clark's combined Phases C and D
  document is in both `Phase C/` and `Phase D/`. Phases A, B, and C have a `Diagrams/` folder.
  They share one format, with no watermark. They were generated on 2026-10-30 for
  upload to the shared Google Drive folder with Sir Pira. The internal Architecture
  Repository Index is in `AI Directory/Generated Outputs/` and is not for submission.
  Older Phase B versions and the Phase B brief and change list also stay there.
  Phase A deliberately keeps three consecutive semesters (Em, 2026-10-30; ISS-009). A2 (Proposal Revision) is still unconfirmed as submitted, and its
  deadline is not recorded. Sir's A2 feedback: reframe around the business's
  WHY before the HOW.
- **Study guides:** as of 2026-10-23, every chapter of Jager's book (1-22)
  has an updated PDF study guide in `Course Files/Updated Study Guides/`,
  in range subfolders. The same folder holds a Book Summary Guide, a
  Connecting the Concepts guide, and a compiled Ch 1-22 PDF. The older Ch
  1-12 guides remain in `Course Files/Study Guides/`.
- **Repo setup:** restructured on 2026-10-16. Laufey's rules are now in
  `CLAUDE.md` and `.claude/rules/`, and its procedures are skills in
  `.claude/skills/`.
- **Submission (set 2026-11-03):** Sir Pira wants all ADM documents and the
  project submitted through a GitHub repo shared with him. The submission is
  the top-level `OSM Architecture/` folder: approved outputs only, by ADM
  phase (`Preliminary`, `Phase A` to `Phase H`, `Requirements Management`),
  plus `Architecture Repository/` with the TOGAF components. It was seeded
  with the v0.1 Phase A-D documents and diagrams (copies; the team's
  originals are unchanged). It holds no README or index, only deliverables
  (`.gitkeep` in empty folders). The root `README.md` explains the project
  and points Sir to it. The GitHub repo was renamed by Em; the local remote
  URL still needs updating.
- **Workflow:** `/spec-driven` (Approach A: chat, design, generate; Approach B:
  design, worksheet in `Users Directory/User Specs/Worksheets/`, review,
  generate) and `/publish-output` (approved draft to `OSM Architecture/`).
  Rules in `.claude/rules/osm-architecture.md`.

## Key Decisions
_(Append, don't overwrite. One entry per decision, with the date and a
one-line reason.)_

- **2026-09-14:** Proceed with the CSA Mentoring Unit as the enterprise.
  Reason: the interview data is rich and already gathered, and switching
  would cost more than any extra complexity would gain.
- **2026-09-14:** Treat the schools' own student-mentor pairing process and
  timing as an out-of-scope external dependency, not something to
  redesign. Reason: the Mentoring Unit has no authority over the schools'
  internal processes.
- **2026-09-14:** Draw the EA boundary around the unit *plus* its direct
  interfaces (schools' coordinators, IT Office, Registrar, HR/Finance,
  governance chain up to ManCom), not the 2-person headcount alone.
  Reason: that is where the real complexity sits.
- **2026-10-16:** No fixed roles or deliverables. The team works from what
  the professor asks for, recorded in `Assignments.md`.
- **2026-10-16:** Study guides go in `Course Files/Study Guides/`, not
  `Generated Outputs`. Laufey asks for the format before generating any
  file, unless it was already given.
- **2026-10-16:** The course books and the interview recording stay in
  the repo (the team's call).
- **2026-10-16:** The seven findings from the First Draft review are
  logged as ISS-001 to ISS-007 and stay open. They were never fixed in the
  team's own documents.
- **2026-10-23:** All new and updated study guides (Ch 1-22 plus the
  whole-book guides) go in `Course Files/Updated Study Guides/`, with no
  "v2" in file names. The original `Study Guides/` folder is left
  untouched. Reason: Em's request.
- **2026-10-23:** A3 scope: the team provides inputs at most, and Laufey
  generates the documents, one per chosen template, using only the necessary
  Phase A-D templates. Reason: Em's answers (his reading of the course; not
  yet confirmed by Sir Pira).
- **2026-10-27:** A3 split: Em = Phase A, Aldrin = Phase B, Clark = Phases
  C and D. Em supplies inputs and Laufey refines and generates, so Em
  learns TOGAF by applying it; Laufey may generate more directly only in an
  emergency or near the deadline. Reason: Em's request. Weekly Claude
  credits are nearly used up, so keep exchanges short and batched.
- **2026-10-29:** Phase B fills only the two Phase B templates (ARS and
  Roadmap). The business models go to the ADD owner through
  `Generated Outputs/2026-10-29 - A3 Phase B - Brainstorm Brief and Handoff.md`.
  Reason: Aldrin's call ("do whatever the template asks for").
- **2026-10-29:** Each school's Mentoring Coordinator decides pairings,
  with same-school mentors preferred. Male and female coordinators split
  the student list, but same-gender mentor pairing is not a rule. The
  target is one centralized workflow with a single pairing register. The
  single platform is a Phase C requirement, and automated matching is a
  later transition step. Reason: Aldrin's input, cross-checked with both
  coordinator interviews.
- **2026-10-29:** The session-log Google Sheet and the coordinators'
  pairing lists are NOT connected. This answers the open "possible
  conflict" and overrides Em's Notes 2. Reason: Aldrin's direct knowledge.
- **2026-10-30:** Missing the 3-session requirement for **two** consecutive
  semesters (not three) affects enrollment. Overrides Em's Notes 2. Phase B
  ARS and the handoff brief are corrected. Reason: matches the RFAW (A1);
  confirmed by Clark (ISS-009).
- **2026-10-30:** The Phase B Roadmap includes *preliminary* drafts of
  3.1 (four capability-based work packages, WP1-WP4), 3.2 and 3.5, marked
  "to be confirmed in Phase E". Reason: Aldrin's call; Laufey had flagged
  them as Phase E work outside A3.
- **2026-10-30:** Edits go into the latest version file. Don't make extra
  version copies. Reason: Aldrin's request.

- **2026-10-30:** A3 Phase A uses three of the five templates (Architecture
  Vision, Statement of Architecture Work, Capability Assessment). There is no
  separate Architecture Definition Document or Communications Plan. Reason: Em's
  call to use only what is necessary.
- **2026-10-30:** Phase A keeps three consecutive semesters and OSM's mentor-change
  flow, and adopts Phase B's 100% targets. Teammates' wording was not edited.
  Reason: Em's decisions; the differences are tracked as ISS-009, ISS-011, ISS-012.
- **2026-10-30:** The mentor approval chain is used as-is for A3 and rechecked later
  (ISS-010). Reason: Em doubts ManCom approves the list, but the SED interview says so.

- **2026-11-03:** Submission is a GitHub repo shared with Sir Pira, front door
  `OSM Architecture/` (approved outputs only). Reason: Sir's instruction.
- **2026-11-03:** No README or index inside `OSM Architecture/`. Reason: Em's
  call; Sir doesn't need them and may deduct for them. Naming and versions
  live in `.claude/rules/osm-architecture.md`.
- **2026-11-03:** Naming. Drafts: `YYYY-MM-DD - A<n> - Phase <X> - <Title> (v2)`.
  In `OSM Architecture/`: `<Title> - v<major>.<minor>`, with no date, assignment
  identifier, or phase code. `v0.x` = submitted draft, `v1.0`+ = approved.
  Reason: Em's call.
- **2026-11-03:** Whole repo stays shared (including Readings and transcripts),
  with `OSM Architecture/` as the front door. Spec Driven Approach (A or B,
  the team's choice) is the standard workflow; worksheets live in
  `Users Directory/User Specs/Worksheets/`. Reason: Em's answers.

## Open Questions
_(Append. Move to Key Decisions once answered.)_

- Whether the CSA Mentoring Unit reads as complex enough for Sir Pira's
  complexity-based grading. The team planned to ask him which dimension of
  complexity he weighs (stakeholder breadth, data/integration, governance
  depth, or technical sophistication).
- How to handle Ms. Kelai's hedged hope that students eventually won't
  need to log sessions. The current guidance is to treat it as a
  long-term aspiration, not a design constraint, because the 3-session
  rule needs ongoing evidence.
- **A2:** the deadline, and whether the summary-format layout came from
  the professor (see `Assignments.md`).
- **A3:** whether Sir Pira set the 2026-10-30 deadline; whether he meant
  "only the necessary templates" and "one document per template"; which
  catalogs and diagrams he expects for Phases C and D; whether A2 was
  submitted; whether he expects any Phase E content (Roadmap 3.1, 3.5) in
  A3.
- **Possible conflict to check** (spotted 2026-10-16): who *manages* the
  tools. `Propsal Summary Format.pdf` says the IST department, and
  `Em's Notes 2.pdf` says the unit. The Sheets-linked part was answered
  on 2026-10-29: they are not linked (see Key Decisions).
- Should the seeded v0.1 files in `OSM Architecture/` be promoted to v1.0
  (approved baseline), and do Sir's reviewers see the repo's transcripts and
  TOGAF PDFs as a problem? (Raised 2026-11-03.)
- **A3:** the Phase B target state and "proposed" success measures still
  need validation with OSM and the sponsor.

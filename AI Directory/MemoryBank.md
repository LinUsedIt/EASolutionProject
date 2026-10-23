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
    transcripts and Em's notes are in the assignment folders.
  - **Size:** 2 staff, one handling monitoring (Ms. Kelai) and one
    handling mentor training. About 1,500–1,600 undergraduates and about
    180 mentors. Sponsor: CSA Executive Director.
  - **Purpose (the WHY, from the 2026-09-28 interview):** the Mentoring
    Program is one of UA&P's hallmarks, supporting the integral
    (holistic) formation of students. The unit exists to keep the program
    uniform and centralized across schools.
  - **Catalyst:** from AY 2026-27, students must have at least 3 mentoring
    sessions per semester. Failing this for three consecutive semesters
    affects enrollment. The requirement is non-negotiable. Participation
    became mandatory under the new university President.
  - **Current pain points:** a large number of mentor-change requests,
    handled by long email chains; dependence on the schools and the
    Registrar for pairings; uncertainty about whether students will log
    their sessions properly.
- **Current focus:** A3, Phases A-D (ADM), due 2026-10-30 (relayed by Em;
  not yet confirmed as Sir's date). Proposed split: Em (Phase A core and
  consistency check), Clark (Phase B and Capability Assessment), Aldrin
  (Communications Plan and Phase C/D artifacts), Architecture Definition
  last and shared. Team input target 2026-10-27. Not yet agreed by the
  team. A2 (Proposal Revision) is still unconfirmed as submitted, and its
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
  submitted. Also whether the team accepts the proposed workload split.
- **Possible conflict to check** (spotted 2026-10-16, not yet logged as an
  issue): `Propsal Summary Format.pdf` §1.1 and §1.3 say the IST
  department creates *and manages* the tools and that the two Google
  Sheets are isolated. `Em's Notes 2.pdf` (from the 2026-09-28 interview)
  says the IT Office has already linked the two Sheets, and that it only
  creates the forms and sheets while the unit manages them.

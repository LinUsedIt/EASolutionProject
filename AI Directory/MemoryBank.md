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
  TOGAF himself. Submission is Friday 2026-10-30. **Phase B is final
  (2026-10-30):** the latest files are the **(v2)** ARS and **(v2)** Roadmap
  in `AI Directory/Generated Outputs/2026-10-30-A3 Phase B/` (the
  unversioned files there are the 10-29 drafts). v2 applies Clark's Phase
  C-D change list, fills ARS 2.3/2.6-2.8 and Roadmap 2.2-2.3, and adds
  preliminary drafts of Roadmap 3.1, 3.2, 3.3.1-3.3.4 and 3.5. **Em: please
  check both v2 files** (and make sure Phase A uses *two* consecutive
  semesters, ISS-009) before submission. The ADD owner has not been
  assigned yet. **Em and Clark:** §7 of the handoff brief (same folder)
  says which Phase B diagrams to reuse; the diagrams are still in
  `Generated Outputs/2026-10-29 - A3 Phase B - Diagrams/`. A2 (Proposal Revision) is still unconfirmed as submitted, and its
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
- **A3:** who writes the Architecture Definition Document (it spans
  Phases B to D)? The Phase B target state and "proposed" success measures
  still need validation with OSM and the sponsor.

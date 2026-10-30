# Session Log: EASolutionProject

One entry per work session with Laufey, newest first. Laufey writes these
with `/log-session`. This file isn't loaded automatically; Laufey reads it
when someone asks about past sessions. The current-state summary is in
`MemoryBank.md`.

Entries marked **(reconstructed)** were written afterwards from git
history and the files in the repo, not from a live session. They record
what was produced, not what was discussed.

## Entry format

Follow this exactly. Write "None" in a field that has nothing; don't drop it.

```
### [YYYY-MM-DD] — [Short topic label]

**Participants:** who was involved (e.g. Em, Clark, Aldrin, Laufey)

**Summary:** a detailed narrative of what was discussed or worked on —
enough that someone reading only this entry understands what happened
without needing the original conversation.

**Decisions Made:**
- 

**Risks / Open Items:**
- 

**Next Steps:**
- 
```

## Entries

### [2026-10-30] — A3 Phase B: change list applied, Roadmap Section 3 drafted, pushed

**Participants:** Aldrin, Laufey

**Summary:** Aldrin pulled Clark's commit `1b73673`. It added the Phase C-D
deliverables (`2026-10-30 - A3 Phase C-D - Architecture Deliverables.docx`
plus diagrams C1-C3), a Phase B change list for Aldrin, and issues ISS-008
and ISS-009. Laufey applied the whole change list to new **(v2)** copies of
the Phase B ARS and Roadmap. The edits were made with python-docx, which was
installed on Aldrin's laptop for this; pip's SSL check failed there, so
Aldrin approved `--trusted-host` for that one install. The changes:
- **Eight corrections.** "Three consecutive semesters" became two (ISS-009).
  The session-log wording now says logs update OSM's master database but
  are not tied to a recorded pairing (ISS-008 context). The stray Roadmap
  note is deleted, and the Roadmap Contents entry now reads "Technology".
- **ARS** 2.3 (S1-S5 service table), 2.6 (TS1-TS6), 2.7 (a new bullet on
  external mentors) and 2.8 were filled in.
- **Roadmap** 2.2 (IS-01 to IS-05) and 2.3 (TA-01 to TA-03) were filled in.
  Six Data, Application and Technology rows were added to the 3.3 gap
  matrix, and the new IDs were added to the 3.4 transitions.
- **Phase E notes.** ARS 2.5 now has a one-line Phase E note.

Aldrin then asked for more Roadmap content, all marked "preliminary, to be
confirmed in Phase E":
- **3.3.1-3.3.4:** one paragraph explaining each column of the gap matrix.
- **3.1 Work Package Portfolio:** four work packages, each delivering one
  capability. WP1 is the Central Pairing Register and Student-List Intake,
  and WP2 is Mentor Change Requests (both Transition 1). WP3 is the Standard
  Pairing Workflow, Capacity and Notifications, and WP4 is Session-Log
  Compliance and Semester Reporting (both Transition 2). BA-08 is not
  scoped. Each subheading 3.1.1-3.1.6 has a table.
- **3.2 Implementation Factor Catalog:** one paragraph each for risks,
  issues, assumptions, dependencies, actions and inputs.
- **3.5:** a table of effectiveness measures, risks R-01 to R-06, and
  candidate SBBs on Google Workspace. The SBBs are taken from Clark's
  Section 4.

Laufey first advised against 3.1 and 3.5, because they are Phase E work
outside A3. Aldrin chose to draft them anyway. All content reuses existing
IDs (BA/IS/TA/SM/S/TS/A/C); nothing new was invented.

Aldrin moved the Phase B files into
`AI Directory/Generated Outputs/2026-10-30-A3 Phase B/` and kept one working
Roadmap (v2, document version 0.3). The ARS (v2) is document version 0.2.
The handoff brief and `MemoryBank.md` now say two semesters. Everything was
committed and pushed as `e25924f`, with a note in MemoryBank asking Em to
check both v2 files.

**Decisions Made:**
- Missing the 3-session rule for two consecutive semesters (not three)
  affects enrollment (ISS-009; Clark confirmed, matches the RFAW).
- Roadmap 3.1 groups the components into four capability-based work
  packages (WP1-WP4), not one per transition or one per component.
- Roadmap 3.1, 3.2 and 3.5 are included as preliminary drafts marked "to
  be confirmed in Phase E". Roadmap 3.2-3.5 are kept in A3 despite being
  Phase E work. Reason: Aldrin's call.
- Updates go into the latest version file, with no extra version copies
  (Aldrin's request).

**Risks / Open Items:**
- The new tables were checked by script only. Their layout in Word has not
  been reviewed.
- ISS-008 (Em's A1 principle wording) and ISS-009 (Phase A must use two
  semesters) stay open until Em confirms.
- Sir Pira has not said whether he expects any Phase E content (3.1, 3.5)
  in A3.
- The targets and the target state still need validation with OSM and the
  CSA Executive Director.

**Next Steps:**
- Em: review the ARS (v2) and the Roadmap (v2), and check that Phase A uses
  two semesters. Then close ISS-009.
- Aldrin: skim both v2 files in Word before submission (2026-10-30).
- Assign the ADD owner.

### [2026-10-29] — A3 Phase B: brainstorm, cross-check, and Phase B documents

**Participants:** Aldrin, Laufey

**Summary:** Aldrin owns Phase B. The template in Aldrin's Downloads is
byte-identical to the one in `Course Files/TOGAF Templates/Phase B - Business Architecture/`
(Architecture Requirements Specification and Architecture Roadmap).
Laufey cross-checked the earlier outputs (A1 revised proposal, SessionLog)
against Em's Notes 2 and both coordinator transcripts, then brainstormed
the Phase B inputs with Aldrin question by question.

Two transcript labels turned out to be wrong:
- `Transcripts/2026-10-16 interview.pdf` is Dr. Olmos, the **SSE** male
  coordinator.
- `Transcripts/Mentoring Coordinator Interview - SSE.pdf` (2026-10-20) is
  actually Sir Lactao, the **School of Education (SED)** coordinator.
- So the SED transcript was already filed, just under the wrong label.

Aldrin decided that Phase B fills only what the two Phase B templates ask
for. The business models (capability map, process diagrams, baseline,
target, gap analysis) are handed to whoever writes the Architecture
Definition Document, through a handoff brief.

Laufey produced, all in `AI Directory/Generated Outputs/`:
- `2026-10-29 - A3 Phase B - Architecture Requirements Specification.docx`
  (8 success measures, 8 business service contracts, guidelines,
  constraints, assumptions; the Phase C and D sections are marked as such)
- `2026-10-29 - A3 Phase B - Architecture Roadmap.docx` (business roadmap
  components BA-01 to BA-08, business rows of the gap matrix, candidate
  transitions; the rest is marked Phase E per the template)
- `2026-10-29 - A3 Phase B - Diagrams/` (capability map, plus Pairing and
  Mentor Change diagrams in baseline and target versions; PNG and SVG)
- `2026-10-29 - A3 Phase B - Brainstorm Brief and Handoff.md` (every
  decision, with its source)

The Word files were built by filling the official templates' XML, because
this laptop has no pandoc, no python-docx, and no pip internet access.
Laufey opened both in Word and checked them through a PDF export. The
diagrams were rendered with headless Edge. The Canva and Figma connectors
failed to connect.

**Decisions Made:**
- Phase B = the ARS and the Roadmap only. The business models go to the
  ADD owner through the handoff brief.
- Capabilities (7): Mentor Sourcing & Approval, Mentor Development,
  Mentee-Mentor Pairing, Pairing Change Management, Session Logging &
  Compliance Monitoring, Program Evaluation & Reporting, Program Promotion.
- School Mentoring Coordinators decide the pairings, with same-school
  mentors preferred. Male and female coordinators split the student list
  by sex. Same-gender mentor pairing is NOT a rule (only an SSE footnote).
- Baseline pairing starts at the Registrar. The list goes to OSM and then
  to the coordinator, or the coordinator asks the Registrar directly. The
  process includes the returning-student survey, the capacity check, the
  overflow step, and the notifications.
- Goal: foster holistic education in line with UA&P's vision. Objective:
  see student growth closely. Drivers: the President's mandate (3-session
  rule), mentoring as a hallmark, and the need for evidence.
- Target: one centralized end-to-end workflow with a single pairing
  register. The single platform is a Phase C requirement. Automated
  matching is a later transition step.
- The two Google Sheets (session log and pairing lists) are NOT connected
  (Aldrin), which overrides Em's Notes 2.
- The old Dragon's Lair platform is left out of the baseline.

**Risks / Open Items:**
- The target state is the team's proposal and has not been validated with
  OSM or the sponsor. All "proposed" success-measure targets need
  confirmation.
- The ADD owner has not been assigned, and the ADD still needs the
  business models from the handoff brief.
- Em should re-check the Sheets claim in Em's Notes 2.
- The transcript files are still mislabeled. They were not renamed,
  because they are the team's files.

**Next Steps:**
- Em and Clark review the Phase B documents before 2026-10-30.
- Clark picks up the single-platform requirement and the
  pairing-register data in Phase C.
- Decide who writes the ADD, using the handoff brief.

### [2026-10-23] — A3 scoping: ADM Phases A-D and workload split

**Participants:** Emmanuel (Em), Laufey

**Summary:** Em asked what the Phase A-D templates in
`Course Files/TOGAF Templates/` are for. Laufey explained that they map to
ADM Phases A (Architecture Vision), B (Business Architecture), C
(Information Systems: data and application), and D (Technology
Architecture), and what each phase means for the CSA Mentoring Unit.
Phase A's templates are Architecture Vision, Statement of Architecture
Work, Capability Assessment, Communications Plan, and Architecture
Definition. Phase B's are Architecture Requirements Specification and
Architecture Roadmap. Phases C and D have no fill-in template, only the
recommended artifacts list in `Architecture Deliverables Phases C and D.docx`.
Laufey read the templates directly and did not yet pull page-level TOGAF
citations from the Readings. Em then confirmed: deadline 2026-10-30; choose
only the necessary templates, as the team did in its scope; one document per
template; the team provides inputs at most, and Laufey generates the
documents. Em's reading of the first two points, and his belief on the third,
are not yet confirmed as Sir Pira's own wording. Laufey proposed a workload
split: Em takes Phase A core (Architecture Vision, Statement of Architecture
Work) and the final consistency check; Clark takes Phase B and the
Capability Assessment; Aldrin takes the Communications Plan and the Phase C
and D artifacts. Architecture Definition is last and shared, because it draws
on B, C, and D. Laufey flagged that Aldrin's Phase C and D work is blocked
until the IT Office ownership conflict is settled, and that the seven-day
window is tight, with an internal input target of 2026-10-27. A3 was updated
in `Assignments.md`. No documents have been generated yet.

**Decisions Made:**
- A3 deadline is 2026-10-30 (relayed by Em; not yet confirmed as Sir's date).
- Use only the necessary Phase A-D templates, not all of them (Em's reading).
- One document per template (Em's belief).
- The team provides inputs at most; Laufey generates the documents.
- Proposed split, pending the team's agreement: Em (Phase A core, final
  consistency check), Clark (Phase B, Capability Assessment), Aldrin
  (Communications Plan, Phase C and D artifacts), Architecture Definition last
  and shared.

**Risks / Open Items:**
- Aldrin's Phase C and D work is blocked by the IST vs. IT Office ownership
  conflict (see MemoryBank Open Questions).
- Clark carries the heaviest load (Phase B plus Capability Assessment).
- The seven-day window is tight, and the school coordinator interview is
  still pending, which feeds the Capability Assessment and Communications Plan.
- Not yet confirmed with Sir Pira: deadline, the template-selection rule, and
  the one-document-per-template format.
- The team has not agreed to the proposed split.

**Next Steps:**
- The team confirms or changes the workload split.
- Confirm the open A3 questions with Sir Pira (deadline, template selection,
  format, and whether he expects specific C and D artifacts).
- Resolve the IST vs. IT Office conflict before Phase C and D inputs.
- Team sends inputs by the internal target of 2026-10-27.
- Laufey drafts the chosen documents once the inputs arrive.

### [2026-10-23] — Full study guide set for Mastering the TOGAF Standard (Ch 1-22)

**Participants:** Emmanuel (assumed from this machine's user folder; correct if wrong), Laufey

**Summary:** The request was to make (1) a summary guide of the whole of
Jager's *Mastering the TOGAF Standard*, (2) detailed guides for every
chapter, including chapters 1-12 that already had guides, and (3) one
guide connecting all the chapters and concepts, with chapter and section
references. Format agreed: PDF. Em then asked for all the new files to go
in a separate folder, `Course Files/Updated Study Guides/`, with no "v2" in
any file name. That is where everything now lives, in range subfolders
`TOGAF Ch1-7/`, `Ch8-9/`, `Ch10-12/`, and `Ch13-22/`. The original guides
in `Course Files/Study Guides/` are untouched. Laufey extracted
the text of all 22 segmented chapter PDFs and read every chapter in full.
It checked page images where the extracted text was scrambled or missing
(Table 2-1, Table 7-4, and several pages of Chapter 12). It wrote each guide
to the make-study-guide template, with page references and Jager's
opinions labelled separately from the Standard, and rendered them with a
new reportlab script. The updated guides also fix the raw `*`/`>` Markdown
showing in the old PDFs. Files created in `Updated Study Guides/`:
- 22 chapter guides (`Chapter N - Title - Study Guide.pdf`) in the four
  range subfolders
- `Mastering the TOGAF Standard - Book Summary Guide.pdf` (7 pp.)
- `Mastering the TOGAF Standard - Connecting the Concepts Study Guide.pdf`
  (12 pp.: nine cross-chapter threads, an ADM backbone table, commonly
  confused pairs, an A-Z concept index, and linking questions)
- `Mastering the TOGAF Standard - Compiled Study Guide (Ch 1-22).pdf`
  (128 pp., with bookmarks)
- A `README.md` in the new folder. `Course Files/Study Guides/README.md`
  now points to it.
Book slips noted inside the guides: Ch 3 p. 48 points to "Chapter 18" for
digital transformation (it is Ch 19); Ch 11 p. 285 says the "2008 eighth
edition" (TOGAF 8 was 2002); Ch 16's mapping section is numbered "16.3.3";
Ch 14 p. 626 mislabels interoperability cell 2A; Ch 22 says "four types
of iteration" (Ch 13 has three ways and four groups).

**Decisions Made:**
- All new guides live in `Course Files/Updated Study Guides/`, with no
  "v2" in names. The old `Study Guides/` folder is left as it was.

**Risks / Open Items (rules):**
- `.claude/rules/file-placement.md` and the make-study-guide skill still
  say study guides go in `Course Files/Study Guides/`. They need updating
  if `Updated Study Guides/` becomes the standard location (proposed, not
  changed).

**Risks / Open Items:**
- The study guides cite the book's page numbers. Claims about the TOGAF
  Standard itself are Jager's account, and were not cross-checked
  against the Standard PDF.

**Next Steps:**
- The team reviews the guides. Commit them when happy (not committed yet).

### [2026-10-16] — Repo restructure: rules, skills, memory, and assignment tracking

**Participants:** Emmanuel (assumed from the git author; correct if
wrong), Claude (setting up the repo, outside the Laufey persona)

**Summary:** Laufey wasn't reliably following its rules because nothing
made Claude Code load `AI Directory/AgentRules.md`. Only a root
`CLAUDE.md` is loaded automatically. The repo was restructured, moving
and adding Markdown files only:
- **Rules:** a new root `CLAUDE.md` holds Laufey's identity, personality,
  responsibilities, team, and repo map, and imports `MemoryBank.md` and
  `Assignments.md`. Topic rules were moved to `.claude/rules/`
  (sources-and-citations, file-placement, file-formats, memory,
  assignments, issue-logging, protected-files, team-and-git).
  `AgentRules.md` was removed, since its content now lives in those files.
- **Skills** in `.claude/skills/`: analyze-document, summarize-document,
  plan-work, make-study-guide (with template.md, matching the existing
  guides), log-session, log-issue, and log-assignment.
- **Subagents** in `.claude/agents/`: togaf-researcher (read-only, cited
  excerpts from the Readings) and deliverable-reviewer (read-only,
  independent review against requirements and TOGAF).
- **Settings:** `.claude/settings.json` makes Claude Code ask before
  editing `CLAUDE.md`, `.claude/`, the team's assignment files, the
  Readings, or the Templates. A `.gitignore` covers personal Claude files,
  `desktop.ini`, and Office lock files.
- **Memory:** `MemoryBank.md` was split. The snapshot, decisions, and open
  questions stay there; session entries moved to this file. The snapshot
  was caught up to A2. Reconstructed entries were backfilled for
  2026-09-15 to 2026-10-15.
- **Assignments:** a new `Assignments.md` records what the professor asks
  for, backfilled with A1 and A2.
- **Issues:** the seven findings from `Issues Log - First Draft Review.md`
  were logged as ISS-001 to ISS-007, all open. That review file was moved
  from the Assignment 1 folder to `AI Directory/Generated Outputs/`.

**Decisions Made:**
- No fixed roles or deliverables. Work follows the professor's requests,
  recorded in `Assignments.md`.
- Study guides are saved in `Course Files/Study Guides/`. Laufey asks for
  the format before generating any file, unless it was already given.
- Books and the interview recording stay in the repo.
- ISS-001 to ISS-007 stay open; they were never fixed.

**Risks / Open Items:**
- A2 deadline not recorded.
- Aldrin's surname not recorded.
- Possible conflict between `Propsal Summary Format.pdf` and
  `Em's Notes 2.pdf` about the Google Sheets (see MemoryBank Open
  Questions).

**Next Steps:**
- Each team member pulls the changes and opens Claude Code from the
  `EASolutionProject` folder.
- Record A2's deadline and requirements with `/log-assignment`.

### [2026-10-13 to 2026-10-15] — Study guides for Chapters 8–12 (reconstructed)

**Participants:** Not recorded (reconstructed)

**Summary:** Reconstructed from file dates; these files weren't
committed as of 2026-10-16. New study guides were created in
`Course Files/Study Guides/`: `TOGAF Ch8-9/` (Chapter 8, Architecture
Governance; Chapter 9, Architecture Capability) and `TOGAF Ch10-12/`
(Chapter 10, Architecture Roles, Skills, and Competencies; Chapter 11,
Architecture Domains; Chapter 12, Architecture Development Method). A
compiled guide, `Mastering the TOGAF Standard - Compiled Study Guide
(Ch 1-12).pdf`, was also created. The TOGAF deliverable templates
(`Course Files/TOGAF Templates/`, one folder per ADM phase) appeared
around the same time.

**Decisions Made:**
- None recorded.

**Risks / Open Items:**
- None recorded.

**Next Steps:**
- Commit the new guides and the templates.

### [2026-10-02] — Assignment 2 materials added (reconstructed)

**Participants:** Emmanuel (git author)

**Summary:** Reconstructed from commit b4bca30. Added the 2026-09-28
follow-up interview transcript (Ms. Nina) and `Propsal Summary Format.pdf`,
a condensed version of the proposal in a four-section layout, to
`Users Directory/Course Assignments/Assignment 2 - Proposal Revision/`.

**Decisions Made:**
- None recorded.

**Risks / Open Items:**
- Unclear whether the summary layout came from the professor.

**Next Steps:**
- None recorded.

### [2026-09-28 to 2026-09-29] — Professor feedback and second interview (reconstructed)

**Participants:** Emmanuel, Clark (interviewers); Laufey (interview guide)

**Summary:** Reconstructed from commit d326381 and the files. Sir Pira
gave feedback on the A1 draft, captured in `Notes from Sir on
revision.pdf`: focus on the business's WHY (purpose, strategy, drivers)
rather than the HOW, look at data, business, tech, and apps, and work
backwards from the problem to strategy. Laufey produced `CSA Mentoring -
Second Interview Guide.docx` in `Generated Outputs`, merging Em's and
Clark's questions and filling gaps against this feedback and the issues
log. The follow-up interview with Ms. Nina took place on 2026-09-28. Em's
notes (`Em's Notes 2.pdf`) record the program goals, the unit's two roles,
mentor training with HR, external mentor sourcing by referral, the IT
Office having linked the two Google Sheets, mentor-change requests as the
biggest current problem, and the 3-session rule as non-negotiable. The
submitted A1 draft (`Enterprise Proposal (Draft)_Datu, Velasco.pdf`) was
also committed.

**Decisions Made:**
- None recorded.

**Risks / Open Items:**
- None recorded.

**Next Steps:**
- Revise the proposal around the WHY (A2).

### [2026-09-17] — Study guides for Chapters 1–7 (reconstructed)

**Participants:** Emmanuel (git author), Laufey

**Summary:** Reconstructed from commit efe94fe. The segmented chapter
PDFs of Jager's *Mastering the TOGAF Standard* were added, and Laufey
generated detailed study guides for Chapters 1–7 in
`Course Files/Study Guides/TOGAF Ch1-7/`.

**Decisions Made:**
- None recorded.

**Risks / Open Items:**
- None recorded.

**Next Steps:**
- None recorded.

### [2026-09-15] — First Draft compiled and reviewed (reconstructed)

**Participants:** Emmanuel (git author), Laufey

**Summary:** Reconstructed from commit f919a07. The four A1 parts
(Executive Summary, Deliverables 1–3) were added under `Parts/`. Laufey
ran a cross-document review that produced `Issues Log - First Draft
Review.md` (7 findings), compiled the parts into
`Assignment 1 - Compiled Enterprise Proposal (Revised).docx`, and wrote
`Assignment 1 - Revision Notes.docx`, which lists a proposed fix for each
of the 7 findings in the compiled version. Per the team (2026-10-16),
those fixes were never adopted in the team's own documents, so the issues
remain open (ISS-001 to ISS-007).

**Decisions Made:**
- None recorded.

**Risks / Open Items:**
- The 7 findings remain open.

**Next Steps:**
- None recorded.

### [2026-09-14] — Deliverable 2 Kickoff and Enterprise-Criteria Verdict

**Participants:** Clark (Deejay Clark Datu, Student B), Laufey

**Summary:** Clark asked Laufey to assess, against the course's
enterprise-selection criteria in `Project - Choosing the Enterprise
Guide.pdf` (Clear Bounded Scope, Explicit Business Catalyst,
Understandable Business/IT Landscape), whether CSA Mentoring Division
actually qualifies. Verdict: passes cleanly on Business Catalyst (the new
mandatory 3-sessions/semester policy) and Understandable Landscape (4
nameable capabilities — Mentor Sourcing & Approval, Pairing, Session
Monitoring/Compliance, Governance — with concrete supporting systems).
Bounded Scope is the one real risk: the Mentoring Unit itself is only 2
employees, well under the guide's 50–1,000-employee sizing anchor.
Recommendation: not to switch enterprises, but to have Deliverable 1's
Boundary & Scope Statement deliberately draw the EA boundary around the
unit *plus* its direct interfaces (schools' coordinators, IT Office,
Registrar, HR/Finance, and the governance chain up to Mancomm) rather
than the 2-person headcount alone, since that's where the real
division-of-labor complexity sits.

Work split confirmed (see Project Snapshot): Clark takes Deliverable 2
(Tailored Architecture Framework), Emmanuel takes Deliverable 1
(Organizational Model for EA). Laufey briefed Deliverable 2
in two parts: a Tailored Enterprise Metamodel (in/out entity pass — e.g.
Organization Unit, Business Actor/Role, Business Process, Data Entity,
and Application Component judged in scope; Technology Component/Network
and Product/Contract judged out of scope, since the unit runs entirely on
Google Workspace SaaS with no infrastructure ownership) and a Tailored
Content Framework (phase-by-phase artifact commitments: Business
Capability Map + a Pairing/Mentor-Change process diagram for Phase B,
Data Entity Diagram for Phase C1, Application Communication Diagram for
Phase C2, a deliberately lightweight Technology Portfolio Catalog for
Phase D). No drafting has started yet — this was scoping only.

**Decisions Made:**
- Deliverable 1's Boundary & Scope Statement should draw the EA boundary
  around the Mentoring Unit plus its direct interfaces, not just the
  unit's 2-person headcount — the fix for the Bounded Scope risk, not a
  reason to reconsider the enterprise choice.
- Work split: Clark owns Deliverable 2; Emmanuel owns Deliverable 1.

**Risks / Open Items:**
- (Carried over) Whether CSA Mentoring Division's complexity will satisfy
  Sir Pira's complexity-based grading — this session's Bounded Scope
  framing fix reduces but doesn't eliminate the risk, since Sir Pira's
  actual weighting is still unconfirmed.

**Next Steps:**
- Draft the real Deliverable 2 Tailored Enterprise Metamodel and Content
  Framework documents.
- Teammate to draft Deliverable 1, including the reframed Boundary &
  Scope Statement.

### [2026-09-14] — Assignment 1 Deep Dive: TOGAF Framing, Scope, and Complexity Concerns

**Participants:** Emmanuel (Student A/B, role unconfirmed), Laufey

**Summary:** Late-night/early-morning session reviewing all Assignment 1
source material for the first time together: the assignment guide
(`Project - Choosing the Enterprise Guide.pdf`), the CSA interview
question guide, the full `2026-09-11 interview transcript.pdf`, and
`Em's Notes.pdf`. Laufey produced a five-part analysis: (1) a summary of
what Assignment 1 actually requires (three Preliminary Phase deliverable
sets — Organizational Model for EA, Tailored Architecture Framework,
Collaborative Foundations/RFAW — all documents, no system-building); (2) a
full profile of CSA's Mentoring Division built from the transcript and Em's
Notes (org structure, ~1,500-1,800 students/~180 mentors, the new
mandatory 3-sessions-per-semester policy as the business catalyst, the
current Google Form/Script/Sheet session-logging pipeline, the two
disconnected databases, and their two self-named pain points: pairing and
monitoring); (3) proposed areas to explore per deliverable, grounded in
specific transcript quotes; (4) a proposed document flow mirroring the
Guide's own deliverable ordering; (5) words of encouragement given the
looming deadline. This analysis was compiled into a `.docx` and saved to
`AI Directory/Generated Outputs/CSA Mentoring Division - Assignment 1
Analysis.docx` (built manually as an OOXML package since no pandoc/python
was available in this environment) — explicitly requested by Emmanuel as
a check that Laufey follows AgentRules §7 (outputs belong in Generated
Outputs, not the assignment folder). Laufey flagged that the transcript's
"this Tuesday" deadline reference (said 2026-09-11) resolves to
**2026-09-15**.

Three substantive concerns were then discussed. First, Emmanuel raised
that school-side pairing turnaround can't be fixed since each school runs
its own process — Laufey agreed this is a genuine external dependency and
recommended documenting it as an explicit out-of-scope constraint (see Key
Decisions) rather than attempting to redesign it, while suggesting
in-scope adjacent improvements (retaining upperclassman pairings across
semesters, standardizing the school-to-unit handoff format, visibility
into which schools have/haven't submitted). Second, Emmanuel asked
whether the assignment is about proposing a solution — Laufey corrected
this: Assignment 1's deliverables are TOGAF **Preliminary Phase** artifacts
(establishing the Architecture Capability), which require identifying
business drivers/problems (needed for the RFAW) but explicitly do NOT
require designing solutions to them (deferred to ADM Phases A–E later in
the semester). Third, Emmanuel raised a grading concern relayed from Sir
Pira (more complex business/solution = higher grade) — Laufey assessed
CSA Mentoring Division as complex enough on stakeholder-breadth,
data-integration, and governance dimensions, but flagged the risk of the
write-up under-presenting that complexity, and recommended asking Sir
Pira directly which dimension of complexity is actually graded. Finally,
Emmanuel asked whether any proposed solution would be rendered pointless
given Ms. Kelai's aside that ideal success looks like students no longer
needing to log sessions at all — Laufey distinguished this hedged,
aspirational comment from Ms. Nina's unhedged, operative success metric
(3 sessions/semester), framed it as an Enterprise/Business Principle
(culture, long-horizon) versus an Architecture Principle (near-term,
actionable) distinction, and concluded it doesn't invalidate near-term
monitoring work — if anything, monitoring data would be the evidence that
such a cultural shift had actually happened.

**Decisions Made:**
- Proceeding with CSA's Mentoring Division (UA&P) as the enterprise;
  not switching despite complexity concerns (see Key Decisions above).
- School-side pairing turnaround treated as an out-of-scope external
  constraint, not a redesign target (see Key Decisions above).

**Risks / Open Items:**
- Assignment 1 deadline is 2026-09-15 — very tight from this session.
- Whether CSA Mentoring Division's complexity will satisfy Sir Pira's
  complexity-based grading; pending his clarification.
- How explicitly to address the "eventually no logging needed" aspiration
  in the Principles Catalog/RFAW.

**Next Steps:**
- Draft Deliverable 1: Boundary & Scope Statement, Stakeholder Map &
  RACI Matrix, Framework Interface Assessment.
- Draft Deliverable 2: Tailored Enterprise Metamodel, Tailored Content
  Framework.
- Draft Deliverable 3: Principles Catalog (3-5 principles), Request for
  Architecture Work.
- Assemble into the proposed document flow (Exec Summary → D1 → D2 → D3
  → Appendix) ahead of the 2026-09-15 deadline.
- Ask Sir Pira what dimension of "complexity" is weighted in grading.

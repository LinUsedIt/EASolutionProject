# Project Brief: EASolutionProject

Shared brief on the team's course project: what the professor has asked for, what has been decided, where the work stands, and what is still open. It is built from the assignment papers and the team's own notes. Anyone may edit; record edits in the Change Log. Requirements live in `AI Directory/Assignments.md` (the record of what Sir Pira asked for) and this file points to it rather than replacing it. Facts about the enterprise are in `AI Directory/OSM Context Brief.md`.

- **Last updated:** 2026-10-30 (first build, by Laufey)
- **Today is the A3 deadline recorded by Em (2026-10-30).** That date is Em's relay, not confirmed as Sir Pira's.

## 1. At a glance

| | |
|---|---|
| Course | IT Elective: Solution Architecture. The subject is Enterprise Architecture (TOGAF), not single-system architecture. |
| Professor | Sir Pira |
| Enterprise | Mentoring Unit / Office of Student Mentoring (OSM), Center for Student Affairs (CSA), University of Asia and the Pacific (UA&P) |
| Team | Emmanuel Velasco ("Em"), Deejay Clark Datu ("Clark"), Aldrin Paltao (surname from the 2026-10-16 transcript header; `MemoryBank.md` still says not recorded). No fixed roles; work follows what Sir asks for. |
| Where it stands | A1 submitted. A2 (proposal revision) in progress, submission unconfirmed. A3 (Phases A-D) in progress, due 2026-10-30 per Em. |
| Final product | An Enterprise Architecture Proposal document outlining the proposed solution for improving the unit (relayed by Em from Sir, in the 2026-09-28 interview, [One source]). |

## 2. The enterprise in five lines

(Full detail and sources: `OSM Context Brief.md`.)

- The OSM is a 2-person unit that implements UA&P's Student Mentoring Program, a university hallmark for holistic formation; it keeps the program uniform across schools.
- Catalyst: from AY 2026-27 students must have at least 3 mentoring sessions per semester. This is non-negotiable. Failing it for consecutive semesters affects enrollment (two per the transcripts; the Memory Bank says three, see open items).
- Scale: about 1,500 to 1,800 students, about 180 mentors, 2 staff, one program across schools. Sponsor is the CSA Executive Director; ManCom approves drastic or institutional changes.
- Named pain points: pairing (late, depends on the Registrar and the schools) and monitoring (will students log sessions?), plus a surge of manual mentor-change requests.
- Tools: Google Sheets, Google Forms, an email script, and email chains, built by the IT Office.

## 3. The assignments

### A1: First Draft Enterprise Proposal (submitted; due 2026-09-15)

- **Source paper:** `Assignment 1/Project - Choosing the Enterprise Guide.pdf`.
- **Enterprise criteria in the guide:**
  - Clear bounded scope (the "town planner" view): complex enough for a recognizable division of labor and several IT systems; the guide's ideal size is 50 to 1,000 employees.
  - An explicit business catalyst, "the Why": "Speak business, not tech" and every technical decision traceable to business strategy.
  - An understandable landscape: 2 to 4 core capabilities and the applications that support them.
- **Deliverables (Preliminary Phase), two-student split in the guide that no longer applies:**
  1. Organizational Model for EA: Boundary and Scope Statement; Stakeholder Map and RACI; Framework Interface Assessment.
  2. Tailored Architecture Framework: tailored metamodel; tailored content framework (which catalogs, matrices, and diagrams the team commits to).
  3. Collaborative Foundations: Principles Catalog (3 to 5 principles, each with Name, Statement, Rationale, Implications; graded on completeness, robustness, understandability, consistency, stability) and a Request for Architecture Work.
- **Submitted draft:** `Enterprise Proposal (Draft)_Datu, Velasco.pdf` and its parts. The seven findings from its review are in `Issues Log - First Draft Review.md` and tracked as ISS-001 to ISS-007 (open, per `MemoryBank.md`).
- **Grading signal relayed by Em (2026-09-14):** Sir's grading favors more complex businesses and solutions.

### A2: Proposal Revision (in progress; deadline unknown)

- **Source paper:** `Assignment 2/Notes from Sir on revision.pdf`. Sir's feedback on the A1 draft, as noted by the team.
- **What Sir said (his points, in his wording where the notes preserve it):**
  - Two things to know. "Know the Business: The WHY." Most papers so far are about the HOW. "That is what the subject is about... But that is not what sir is looking for." Understand the business: not the problems, but the strategy and why they exist. "Change mindset to strategy!!" What drives the company? "What do they want to happen?"
  - Look at what they have: data, business, tech, apps.
  - Goal, business, and purpose of the unit; technology comes only after strategy, capability, and gaps.
  - Look at the 4 architectures and the target for each, so they move the unit from point A to point B.
  - "Given the problem, you have to backtrack: pathfinding."
  - Applied to mentoring, his notes record: they exist because university policy mandates them; they get mentors (professors) from different schools or externally ("Do they train them????"); schools assign mentors to students; the problem is low participation, solved by the mandatory 3-session policy with consequences; sessions monitored via a Google Form with a mentor confirmation workflow and Google Sheets; data integrity by manual checking; and a pending question on why participation matters to the unit ("Is it because they are losing money? (them paying mentors?)").
- **Team file that looks like the A2 deliverable:** `Propsal Summary Format.pdf`. Its cover reads "Enterprise Architecture Preliminary Phase Proposal, Prepared by Deejay Clark Datu and Emmanuel II Velasco, October 2026". That makes it the **team's own condensed draft**, not a format sheet from Sir. Whether Sir set its four-section layout is still an open question in `Assignments.md`. Sections: (1) Enterprise Boundary and Problem Authenticity; (2) Organizational Model for EA; (3) Tailored Architecture Framework; (4) Collaborative Foundations and Evidence.
- **Gap against Sir's feedback:** that draft still opens with scope and failure modes (how) and has no strategy or WHY section, no baseline and target for the four architectures, and no pathfinding from problem to strategy. The WHY material now exists in the 2026-09-28 interview (`OSM Context Brief.md`, section 1).
- **Process expectation relayed by Em:** Sir said the project will go through several iterations and is not weighted until the final product; Em expected one or two more revisions and then the next phase (I2 [71:08]-[71:39], [One source]).

### A3: Phases A-D (Architecture Vision through Technology Architecture)

- **Deadline:** 2026-10-30 (relayed by Em; not confirmed as Sir's date).
- **What is recorded** (`Assignments.md`, A3):
  - Do ADM Phases A to D using the official templates in `Course Files/TOGAF Templates/`.
  - Choose only the necessary templates (Em's reading; not confirmed as Sir's).
  - One document per template (Em's belief; not confirmed).
  - Sir recommended getting the perspectives of the Mentoring Coordinators and Mentors. This is a recommendation, not a hard requirement. Sir's own words as relayed to Dr. Olmos: he "wants us to expand a bit more on our paper scope to try and include what the mentoring coordinators and mentors want for the program", possibly useful "in developing a strategy for the OSM to use" (I3 [51:15]).
  - The team supplies inputs at most; Laufey generates the documents (Em, 2026-10-23). The split set on 2026-10-27: Em = Phase A, Aldrin = Phase B, Clark = Phases C and D. Em supplies inputs and Laufey refines and generates, so Em learns TOGAF by applying it; Laufey may generate more directly only in an emergency or near the deadline.
- **Also noted in interviews:** Sir recommends continuing into a development phase after the conceptual work, if feasible (I1 [35:00]); the OSM was open to that.

## 4. A3 deliverable map

The templates are in `Course Files/TOGAF Templates/`. The Guide's roadmap (Table 54, from the TOGAF Standard 10th Edition Pocket Guide) maps phases to deliverables.

| Phase | Templates available in the repo | Owner | Status found |
|---|---|---|---|
| A: Architecture Vision | Architecture Vision; Statement of Architecture Work; Capability Assessment; Communications Plan; Architecture Definition | Em | `Users Directory/User Specs/Phase A - Inputs.md` exists with `status: draft`. It marks Vision, Statement of Architecture Work, and Capability Assessment as needed; Communications Plan and Architecture Definition as skipped. The template for each is a separate `.docx`. Many items are prefilled from the Memory Bank and the 2026-10-20 (School of Education) interview and are awaiting Em's answers. |
| B: Business Architecture | Architecture Requirements Specification; Architecture Roadmap | Aldrin | No spec found. |
| C: Information Systems Architecture | None as fill-in; `Architecture Deliverables Phases C and D.docx` lists recommended artifacts | Clark | No spec found. |
| D: Technology Architecture | Same file as Phase C | Clark | No spec found. |

(Status above is what I found in the repo on 2026-10-30; it may lag the team's work elsewhere.)

**What the team committed to in the draft proposal (Section 3.2):** 11 artifacts across Phases A-E, using ArchiMate for most diagrams and BPMN for business processes:

- Phase A: Architecture Vision Diagram
- Phase B: Business Capability Map; Capability, Process, and Organization Unit Matrix; Business Process Diagrams (Pairing and Change of Mentor)
- Phase C: Data Entity Diagram; Data Entity to Organization Unit Matrix; Application Portfolio Catalog; Application Communication Diagram; Application to Data Entity Matrix
- Phase D: Technology Service Catalog
- Phase E: Architecture Roadmap incorporating Gap Analysis

A3 stops at Phase D, so the Phase E roadmap is outside A3 unless Sir says otherwise (the Architecture Roadmap template sits in the Phase B folder in this repo).

**Diagrams listed in the Guide by phase** (the Guide's list is the closest thing to a statement of what Sir expects for C and D; it is not marked as a requirement):

- A: stakeholder map, architecture vision diagram, value chain or value stream view
- B: business capability map, business process diagrams, organization or role structure diagram, business interaction views
- C1 (Data): data entity diagram or logical data model, data service diagrams, data flow or mapping
- C2 (Applications): application landscape, application interaction, application-to-capability mapping
- D: technology architecture or platform view, technology capabilities map, deployment and hosting view, integration or communications topology

The Guide's "what is required vs optional" note: required for understanding and approval are the diagrams that show baseline versus target and the main relationships (capabilities to processes, applications to capabilities, data entities to applications, technology platforms to applications and integration, plus migration sequencing); detailed BPMN and granular deployment diagrams are optional unless the audience needs them.

## 5. What Sir wants: working summary

Read this before drafting anything for Sir.

1. **WHY and strategy before HOW and technology.** Start from why the unit exists and what it wants to happen (S).
2. **Trace everything back to the business.** "Speak business, not tech"; every technical decision traceable to business strategy (A1 guide).
3. **Four architectures, baseline to target.** For each (business, data, application, technology) say where the unit is, where it should be, and the gap. "Pathfinding": from the problem, backtrack to the strategy (S).
4. **Complexity counts.** His grading favors more complex businesses and solutions (relayed by Em). Whether he weighs stakeholder breadth, data and integration, governance depth, or technical sophistication is an open question.
5. **Definitions get probed.** Expect him to ask "what does holistic mean?" then "what does upstanding mean?" and so on until measurable (I2 [22:30]-[23:01]). Prepare measurable definitions.
6. **He knows the mentoring process.** He built the old mentoring portal and the OSM staff described this as a "double-edged sword" (I1 [49:42]; N1). Details must be accurate.
7. **Include coordinator and mentor perspectives** (recommended).

## 6. Decisions on record

(From `MemoryBank.md`; append there, not only here.)

- 2026-09-14: CSA Mentoring Unit is the enterprise (rich data already gathered; switching would cost more than it gains).
- 2026-09-14: The schools' own pairing process and timing are an external dependency and out of scope (the unit has no authority over it).
- 2026-09-14: The EA boundary is the unit plus its direct interfaces (schools' coordinators, IT Office, Registrar, HR/Finance, governance up to ManCom), not just the 2-person headcount.
- 2026-10-16: No fixed roles or deliverables; follow what Sir asks for (`Assignments.md`).
- 2026-10-16: The course books and the interview recording stay in the repo.
- 2026-10-16: The seven First Draft findings are logged as ISS-001 to ISS-007 and stay open.
- 2026-10-23: Study guides (Ch 1-22 plus whole-book guides) go in `Course Files/Updated Study Guides/`.
- 2026-10-23: A3 scope: team provides inputs at most; Laufey generates one document per chosen template, using only the necessary Phase A-D templates.
- 2026-10-27: A3 split: Em = Phase A, Aldrin = Phase B, Clark = Phases C and D; coach mode (Em supplies inputs and Laufey refines); keep exchanges short and batched because weekly credits are nearly used up.
- 2026-10-30: The team keeps `OSM Context Brief.md` and `Project Brief.md` in the repo as shared markdown source-of-truth files (Em's choice).

## 7. Open questions and risks

**Confirm with Sir Pira (from `Assignments.md`):**

- Is this officially A3, and is 2026-10-30 his date?
- Is it only the necessary templates, and one document per template?
- Which catalogs, matrices, and diagrams does he expect for Phases C and D (no fill-in templates exist)?
- Was A2 submitted? What is its deadline, and did he set the four-section layout of `Propsal Summary Format.pdf`?
- Whether the CSA Mentoring Unit reads as complex enough for his complexity-based grading.

**Contradictions found in the team's own material** (details in `OSM Context Brief.md`, section 13):

- The 3 consecutive semesters in `MemoryBank.md`, the draft proposal, and `Phase A - Inputs.md` vs two consecutive semesters in the transcripts and Em's notes. Phase A text will be wrong if this is not settled.
- The Phase A inputs sheet attributes the Dr. Lactao findings (School of Education coordinator, recorded 2026-10-20) to the SSE interview; the SSE coordinator interview is the 2026-10-16 one with Dr. Olmos. The file `Mentoring Coordinator Interview - SSE.pdf` is Dr. Lactao's.
- The draft proposal says the two Google Sheets are isolated and that IST creates and manages the tools; by 2026-09-28 the IT Office had linked the sheets and the unit manages the tools (`MemoryBank.md` open question).
- Scope tension (ISS-001): the 2026-09-14 decision treats pairing as an out-of-scope external dependency, but the draft proposal commits to a Business Process Diagram for pairing and change of mentor in Phase B. The change-of-mentor process is the unit's own and its biggest current pain; pairing itself is the schools'. Decide the line before Aldrin starts Phase B.
- "SSE" is expanded two ways in the repo.

**Risks:**

- A3 is due today and only the Phase A spec was found (still a draft). Phases B, C, and D have no spec in `Users Directory/User Specs/`. If they exist elsewhere, tell Laufey.
- Phases C and D rest on thin data evidence: the OSM data (pairing database fields; session log fields), the tools, and the integrations are known only from interviews, and the IT Office has not been interviewed.
- The mentor interviews are not done, so Sir's recommendation on perspectives is only half met.
- The team's Claude credits are nearly used up for the week; plan batched requests.

## 8. Where things live

| What | Where |
|---|---|
| What Sir asked for | `AI Directory/Assignments.md` |
| Project snapshot, decisions, open questions | `AI Directory/MemoryBank.md` |
| Session history | `AI Directory/SessionLog.md` |
| OSM facts with sources | `AI Directory/OSM Context Brief.md` |
| Team inputs for deliverables | `Users Directory/User Specs/` (Laufey acts only on `status: ready`) |
| Issues | `Users Directory/Issues/CurrentIssues.md` and `CurrentIssuesList.csv` |
| Official templates | `Course Files/TOGAF Templates/` (read-only) |
| TOGAF sources Laufey may cite | `Course Files/Readings/` |
| Study guides | `Course Files/Updated Study Guides/` (Ch 1-22 and whole-book guides); older Ch 1-12 in `Course Files/Study Guides/` |
| Team drafts, notes, transcripts | `Users Directory/Course Assignments/` (read-only for Laufey) |

## Change Log

| Date | Who | What changed |
|---|---|---|
| 2026-10-30 | Laufey (requested by Em) | First build from the A1 guide, Sir's revision notes, the team's summary proposal, `Assignments.md`, `MemoryBank.md`, and `Phase A - Inputs.md`. |

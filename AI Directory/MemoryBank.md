# Memory Bank — EASolutionProject

Persistent project memory. **Laufey must update this file after every
session** with a detailed summary — see `AgentRules.md` §7 for the rule,
and the entry format below for exactly how.

## Project Snapshot
_(High-level, current-state facts — overwrite in place as things change,
don't append duplicates here.)_

- **Project:** EASolutionProject
- **Course:** IT Elective: Solution Architecture (content is Enterprise
  Architecture — see `AgentRules.md`)
- **Team:** Deejay Clark Datu ("Clark") — Student B, Framework & Metamodel
  Architect, leads Deliverable 2. Emmanuel Velasco — Student A,
  Organizational Architect, leads Deliverable 1.
- **Chosen enterprise:** the **Mentoring Division, Center for Student
  Affairs (CSA), University of Asia and the Pacific (UA&P)**. Stakeholder
  interview conducted 2026-09-11 (Ms. Nina and Ms. Kelai, Operations
  Coordinators). As of 2026-09-14 the team has committed to proceeding
  with this enterprise for Assignment 1 and will not swap it out over
  complexity concerns — see Key Decisions. All source material lives in
  `Users Directory/Course Assignments/Assignment 1 - First Draft Enterprise
  Proposal/` (assignment guide, interview questions, interview transcript,
  Em's Notes).
- **Current phase / focus:** Drafting Assignment 1 ("First Draft Enterprise
  Proposal") — Preliminary Phase deliverables (Organizational Model for
  EA, Tailored Architecture Framework, Principles Catalog + Request for
  Architecture Work). **Deadline: 2026-09-15** (stated as "this Tuesday"
  in the 2026-09-11 interview). Work is split: Clark owns Deliverable 2
  (Tailored Architecture Framework), Emmanuel owns Deliverable 1
  (Organizational Model for EA).

## Key Decisions
_(Running list — append, don't overwrite. One line per decision, with the
date and a one-line reason.)_

- **2026-09-14:** Proceeding with CSA's Mentoring Division (UA&P) as the
  enterprise for Assignment 1, resolving the prior open question. Reason:
  interview data is rich and already gathered; submission is an early,
  low-stakes draft in an iterative process, so switching now would cost
  more than any complexity gained. Not treated as irreversible — could
  still be revisited in a later draft if it proves too thin, but not
  planned.
- **2026-09-14:** School-side student-mentor pairing turnaround (each
  school's own coordinator process/timing) will be documented as an
  out-of-scope external dependency/constraint in the Boundary & Scope
  Statement and RFAW, not a target for redesign. Reason: the Mentoring
  Unit itself has no authority over school-internal pairing processes;
  proposing to fix it would exceed the EA team's actual mandate and
  visibility.

## Open Questions / Risks / Next Steps
_(Running list — append. Cross out or move to Key Decisions once resolved.)_

- Whether CSA Mentoring Division's complexity (2-person unit, lightweight
  Google Workspace tooling) will read as sufficiently complex for grading,
  given Sir Pira's stated complexity-based grading approach (more complex
  business/solution = higher grade). Team plans to ask Sir Pira directly
  what dimension of complexity is weighted (org/stakeholder breadth,
  data/integration challenges, governance depth, or technical
  sophistication) rather than guess.
- Whether/how to explicitly address Ms. Kelai's hedged aspiration
  ("probably won't need logging" once mentoring's value is internalized)
  in the Principles Catalog or RFAW — current guidance given: treat it as
  a forward-looking note, not a design constraint, since the operative,
  unhedged success metric (3 sessions/semester, per Ms. Nina) requires
  ongoing compliance evidence while the policy is enforced.

## Session Log

Every session gets its own entry, most recent at the top, in this exact
format:

```
### [YYYY-MM-DD] — [Short topic label]

**Participants:** who was involved (e.g. Student A, Student B, Laufey)

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

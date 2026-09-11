# EASolutionProject

> **Course:** IT Elective: Solution Architecture — despite the name, this
> course is about **Enterprise Architecture (EA)**, and that's the lens all
> deliverables in this repo are built around.
> **Team:** Student A (Organizational Architect) · Student B (Framework &
> Metamodel Architect)
> **Status:** In progress

## 1. Project Description

This repository is the working space for a two-student practicum in
Enterprise Architecture, built around the TOGAF® Standard. The goal is to
apply the TOGAF Architecture Development Method (ADM) to a **theoretical,
mocked-up enterprise** rather than a real organization, so the team can
practice the discipline end-to-end without the constraints of a live
company.

The enterprise itself is chosen to fit a specific profile so the exercise
stays realistic and tractable:

- **Size:** a mid-sized regional business (roughly 50–1,000 employees) —
  e.g. a wholesale distributor, a regional hospital/clinic, or a logistics
  provider — large enough to have a real division of labor and multiple IT
  systems, but small enough to model in full.
- **A clear business catalyst:** a concrete driver such as a shift to online
  sales, a legacy-to-cloud migration, or post-merger systems integration,
  so every architectural decision can be traced back to a business reason.
- **A legible business/IT landscape:** at least 2–4 recognizable business
  capabilities (e.g. Customer Management, Logistics) and the applications
  that support them.

> **TODO:** once the team finalizes the enterprise, log it in
> `AI Directory/MemoryBank.md` and add a profile write-up under
> `Users Directory/Course Assignments/EASolutionProject/`.

## 2. What This Project Covers (TOGAF)

The work is scoped to TOGAF's **Preliminary Phase** — establishing the
Architecture Capability before the ADM cycle proper (Phases A–H) begins —
split into three deliverables:

### Deliverable 1 — Organizational Model for EA (Student A lead)
- **Boundary and Scope Statement** — which departments, organizational units,
  and geographic locations the EA team's work covers.
- **Stakeholder Map & RACI Matrix** — key stakeholders (CEO, CFO, CIO,
  business unit heads), their concerns, and who is Responsible, Accountable,
  Consulted, or Informed for ADM activities.
- **Framework Interface Assessment** — how the EA team's cadence interacts
  with existing frameworks already in use (e.g. Agile/Scrum, ITIL).

### Deliverable 2 — Tailored Architecture Framework (Student B lead)
- **Tailored Enterprise Metamodel** — the standard TOGAF Foundation
  Metamodel, pared down to the entities that are actually relevant.
- **Tailored Content Framework** — which catalogs, matrices, and diagrams
  from the Extended Content Framework the team commits to producing in
  later ADM phases.

### Deliverable 3 — Collaborative Foundations (joint)
- **Principles Catalog** — 3–5 foundational Enterprise and Architecture
  Principles, each written to the TOGAF four-part template (Name,
  Statement, Rationale, Implications).
- **Request for Architecture Work** — the formal brief from the business
  sponsors that triggers the ADM cycle.

## 3. How the Repo Functions

### Structure
```
AI Directory/
    AgentRules.md    — reference materials, context, and rules the AI follows
    Workflows/
        Brainstorming.md
    MemoryBank.md     — running project context across sessions
    Generated Outputs/ — any file outputs the AI makes

Users Directory/
    Course Assignments/  — assignments divided into folders, each holding
                            drafts/final outputs
    Issues/
        CurrentIssues.md      — list of current issues, open or resolved
        CurrentIssuesList.csv

Course Files/
    Readings/
    AI Explanations/  — write-ups explaining a concept or problem, made
                         whenever a student asks the AI to explain one

README.md
```

The repo is organized around **who's using each part**: the `AI Directory`
holds what an AI assistant needs to work here consistently, the
`Users Directory` holds the assignment work and issue tracking, and
`Course Files` holds shared course material.

### Reference materials the AI should use

For TOGAF questions or drafting, the AI should ground its answers only in
the three sources kept under `Course Files/Readings/`:

1. The TOGAF® Standard, 10th Edition
2. The TOGAF® Enterprise Architecture Foundation Study Guide
3. Mastering the TOGAF® Standard (Eric Jager)

The assignment/guidelines document should **not** be cited as a TOGAF
source — it's instructions for the assignment, not TOGAF content itself.

### Workflow
No specific workflow is defined yet. `AI Directory/Workflows/` exists for
whenever the team standardizes a repeatable process (e.g. brainstorming or
review routine); until then, work proceeds ad hoc.

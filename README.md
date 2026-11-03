# OSM Architecture: Enterprise Architecture for the Mentoring Unit, UA&P

**Course:** IT Elective: Solution Architecture (Enterprise Architecture)
**Professor:** Sir Pira
**Team:** Emmanuel Velasco, Deejay Clark Datu, Aldrin

## About the project

This repository holds an Enterprise Architecture developed with the TOGAF®
Standard's Architecture Development Method (ADM). The enterprise is the
**Mentoring Unit (Office of Student Mentoring, OSM) of the Center for Student
Affairs (CSA), University of Asia and the Pacific (UA&P)**.

The Mentoring Program is one of UA&P's hallmarks, supporting the integral
formation of students. The unit keeps the program uniform and centralized
across schools. From AY 2026-27, every student must have at least 3
mentoring sessions per semester, and missing this for two consecutive
semesters affects enrollment. The architecture moves the unit from its
current way of working (long email chains for mentor changes, reliance on
schools and the Registrar for pairings, uncertain session logging) to a
centralized, trackable mentoring workflow. The architecture is built from
interviews with the unit's operations staff and with School Mentoring
Coordinators.

## Where to look: `OSM Architecture/`

**The submission is the [`OSM Architecture/`](OSM%20Architecture/) folder.**
Everything the team has approved is there, organized by ADM phase:

| Folder | What it holds |
|---|---|
| [`Preliminary/`](OSM%20Architecture/Preliminary) | Preliminary Phase outputs |
| [`Phase A - Architecture Vision/`](OSM%20Architecture/Phase%20A%20-%20Architecture%20Vision) | Architecture Vision, Statement of Architecture Work, Capability Assessment, and diagrams |
| [`Phase B - Business Architecture/`](OSM%20Architecture/Phase%20B%20-%20Business%20Architecture) | Architecture Requirements Specification, Architecture Roadmap, business diagrams |
| [`Phase C - Information Systems Architectures/`](OSM%20Architecture/Phase%20C%20-%20Information%20Systems%20Architectures) | Data and Application architecture deliverables and diagrams |
| [`Phase D - Technology Architecture/`](OSM%20Architecture/Phase%20D%20-%20Technology%20Architecture) | Technology architecture deliverables |
| `Phase E` to `Phase H`, `Requirements Management/` | For later phases; empty until that work starts |
| [`Architecture Repository/`](OSM%20Architecture/Architecture%20Repository) | The TOGAF Architecture Repository, organized by its components: Architecture Metamodel, Architecture Landscape (Strategic, Segment, Capability), Solutions Landscape, Architecture Requirements Repository, Reference Library, Standards Library, Governance Repository, Architecture Capability |

Phase folders hold the deliverables. The Architecture Repository holds the
reusable and governing assets behind them. Diagrams are in each phase's
`Diagrams/` subfolder (PNG and SVG). Files are named
`<Title> - v<major>.<minor>`: `v0.x` is a draft submitted for review,
`v1.0` and above are approved baselines, and superseded versions move to an
`Archive/` folder.

## Other folders (the team's working files)

| Folder | What it is |
|---|---|
| `AI Directory/` | Working memory and generated drafts of the AI assistant |
| `Course Files/` | Course readings, TOGAF templates, and study guides |
| `Users Directory/` | The team's own drafts, notes, interview material, specs, and issue tracker |
| `.claude/`, `CLAUDE.md` | Configuration for the team's AI assistant, Laufey (Claude Code) |

## How the team works (brief)

Work follows a **Spec Driven Approach**: the design is agreed first (in
chat, or through a filled-in worksheet), then the documents are generated.
Drafts are reviewed by the team, and only approved outputs are saved into
`OSM Architecture/`. Open Claude Code from this repository's root folder so
it loads the assistant's rules; its commands (`/spec-driven`,
`/publish-output`, `/analyze-document`, `/plan-work`, `/log-session`, and
others) are in `.claude/skills/`. To change the assistant's rules, edit
`CLAUDE.md` or `.claude/rules/`, or ask it to propose a change.

> TOGAF® is a registered trademark of The Open Group.

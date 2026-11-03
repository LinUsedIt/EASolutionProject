# OSM Architecture

An Enterprise Architecture for the **Mentoring Unit (Office of Student
Mentoring, OSM), Center for Student Affairs (CSA), University of Asia and the
Pacific (UA&P)**, developed with the TOGAF® Standard's Architecture
Development Method (ADM).

**Course:** IT Elective: Solution Architecture (Enterprise Architecture)
**Professor:** Sir Pira
**Team (Group 7):** Emmanuel Velasco, Deejay Clark Datu, Aldrin

## About the project

The Mentoring Program is one of UA&P's hallmarks, supporting the integral
(holistic) formation of students. The Mentoring Unit keeps the program
uniform and centralized across schools. It is a two-person unit serving about
1,500 to 1,600 undergraduates and about 180 mentors, and it works with the
schools' Mentoring Coordinators, the IT Office, the Registrar, and the CSA
governance chain.

**Why now:** from AY 2026-27, every student must have at least 3 mentoring
sessions per semester. Missing this for two consecutive semesters affects
enrollment.

**The problem today:** mentor-change requests are handled through long email
chains, pairings depend on the schools and the Registrar, and it is uncertain
whether students will log their sessions properly.

**What this architecture does:** it describes the unit's business, data,
application, and technology architectures and a path from the current state
to a centralized, trackable mentoring workflow. It is based on interviews with
the unit's operations staff and with School Mentoring Coordinators.

## Folder structure

Each folder maps to a part of the ADM. The documents are the deliverables;
the Architecture Repository holds the reusable and governing assets behind
them.

| Folder | What it holds |
|---|---|
| `Preliminary/` | Preliminary Phase outputs |
| `Phase A - Architecture Vision/` | Architecture Vision, Statement of Architecture Work, Capability Assessment, and diagrams |
| `Phase B - Business Architecture/` | Architecture Requirements Specification, Architecture Roadmap, and business diagrams |
| `Phase C - Information Systems Architectures/` | Data and Application architecture deliverables and diagrams |
| `Phase D - Technology Architecture/` | Technology architecture deliverables |
| `Phase E` to `Phase H`, `Requirements Management/` | Later ADM phases; empty until that work starts |
| `Architecture Repository/` | The TOGAF Architecture Repository, with one folder per component: Architecture Metamodel, Architecture Landscape (Strategic, Segment, Capability), Solutions Landscape, Architecture Requirements Repository, Reference Library, Standards Library, Governance Repository, Architecture Capability |

Diagrams are in each phase's `Diagrams/` subfolder, as PNG and SVG. Phase C
and Phase D share one combined document, which appears in both folders.

## File names and versions

Files are named `<Title> - v<major>.<minor>`, for example
`Architecture Vision - v0.1.docx`.

- `v0.x`: a draft submitted for review.
- `v1.0` and above: an approved baseline. `v1.1` is a small revision and
  `v2.0` a major rework.
- When a new version is approved, the previous one moves to an `Archive/`
  folder in the same phase.

TOGAF® is a registered trademark of The Open Group.

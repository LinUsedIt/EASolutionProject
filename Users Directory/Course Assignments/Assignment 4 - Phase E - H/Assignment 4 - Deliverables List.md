# Assignment 4: Deliverables List (Phases E to H)

**Task (relayed by Em, 2026-11-10):** finish the remaining ADM phases.
**Deadline:** 2026-11-27 (relayed by Em, 2026-11-10; not yet confirmed as Sir's date).
**Prepared:** 2026-11-10, by Laufey. This is a **proposal** for the team to
confirm, not something Sir Pira specified. Sir's actual wording is not yet
recorded; see "Questions for Sir Pira" at the end.

Source of the template list: `Course Files/TOGAF Templates/` (one folder per
phase). Phase E artifacts come from Jager 2025, Ch. 7, Table 7-4, p. 163.
Jager also notes that creating every artifact in the Standard "is by no means
a necessity" (Ch. 7, pp. 155, 157), which supports the team's earlier choice
to use only what is necessary.

## 1. Proposed deliverables

"Include" means I recommend it; "Decide" means the team should choose.

### Phase E: Opportunities and Solutions

| # | Deliverable | Source | Recommendation | Notes |
|---|---|---|---|---|
| E1 | Implementation and Migration Plan | Template (stored in the Phase E folder) | **Include** | The main Phase E output: work packages, projects, sequencing, resources. Builds on the preliminary WP1 to WP4 in the Phase B Roadmap. |
| E2 | Architecture Roadmap (update) | Existing `Architecture Roadmap - v0.1` (Phase B folder) | **Include** | The Roadmap's sections 3.1, 3.2, and 3.5 were drafted early and marked "to be confirmed in Phase E". Finalize them here and issue a new version. |
| E3 | Project Context Diagram | Jager 2025, Ch. 7, p. 163 | **Include** | One diagram per work package or for the whole set. |
| E4 | Benefits Diagram | Jager 2025, Ch. 7, p. 163 | **Include** | Links the work packages to benefits, for example meeting the 3-session requirement. |

### Phase F: Migration Planning

| # | Deliverable | Source | Recommendation | Notes |
|---|---|---|---|---|
| F1 | Implementation Governance Model | Template (Phase F folder) | **Include** | Who oversees implementation and how. Fits a two-person unit with the Architecture Board role played by CSA leadership. |
| F2 | Architecture Contract | Template (Phase F folder) | **Decide** | Useful if another party (the IT Office or a vendor) will build the platform. If no implementer is known, a short contract for the single platform work package is enough. |
| F3 | Architecture Building Blocks | Template (Phase F folder) | **Decide** | Phases B to D already describe building blocks. Either fill the template as a consolidated catalog, or state that Phases B to D cover it. |

The Implementation and Migration Plan (E1) is finalized in Phase F as well, so
update it rather than writing a second plan.

### Phase G: Implementation Governance

| # | Deliverable | Source | Recommendation | Notes |
|---|---|---|---|---|
| G1 | Compliance Assessment | Template (Phase G folder) | **Include** | Shows how the platform and processes would be checked against the architecture. Needs a scenario (for example the pairing register). |
| G2 | Solution Building Blocks | Template (Phase G folder) | **Decide** | These name specific products or components. The team has not chosen a platform, so this may stay at a high level or be skipped. |

### Phase H: Architecture Change Management

| # | Deliverable | Source | Recommendation | Notes |
|---|---|---|---|---|
| H1 | Change Request | Template (Phase H folder) | **Include** | Fill with one worked example (for example a new school joining the program, or a change to the 3-session rule). |
| H2 | Requirements Impact Assessment | Template (Phase H folder) | **Include** | Pairs with H1: what the example change does to existing requirements. |

### Requirements Management (runs through every phase)

| # | Deliverable | Source | Recommendation | Notes |
|---|---|---|---|---|
| R1 | Requirements update | Existing `Architecture Requirements Specification - v0.1` (Phase B folder) | **Include** | No template for this phase. Update the ARS where Phases E to H add or change requirements, and issue a new version. |

### Cross-cutting (every phase)

| # | Task | Notes |
|---|---|---|
| X1 | TOGAF Enterprise Architecture Checklist | **Team-written and team-maintained**, not by Laufey (Sir Pira, relayed 2026-11-10). Update it each time a phase changes. |
| X2 | Revisit Phases A to D | Update earlier documents when E to H expose gaps. Open issues ISS-009 to ISS-012 and ISS-010 (approval chain) are candidates. |
| X3 | Independent review | Run `/analyze-document` with the `deliverable-reviewer` agent across the set before publishing. |
| X4 | Publish approved outputs | `/publish-output` to `OSM Architecture/`, then the subtree push to G7-Repository. |

**Counts:** 10 documents or diagrams recommended (E1 to E4, F1, G1, H1, H2, plus
the E2 and R1 updates), and 3 decisions (F2, F3, G2).

## 2. Do we need to meet the OSM again?

**Short answer: yes, one meeting, and it is worth doing.** Phases A to D
were mostly descriptive and could be built from the interviews. Phases E to H
ask for *decisions and commitments* that only the unit can make, and the
current evidence does not cover them.

What the interviews do **not** tell us yet (from `MemoryBank.md` and the
Phase B open questions):

| Gap | Needed for |
|---|---|
| Priorities, sequencing, and realistic timing of the four work packages, given the AY 2026-27 deadline | E1, E2, E3 |
| Resources, budget, and who would own and run a single platform (the unit or the IT Office / IST). The earlier "who manages the tools" conflict is still open | E1, F1, F2 |
| Target state and "proposed" success measures, flagged as needing validation with OSM and the sponsor | E4, G1 |
| How decisions get approved and by whom (ManCom role is unverified, ISS-010) | F1, H1 |
| What the unit does today when a rule or process changes (who decides, how it is communicated) | H1, H2 |
| Whether mentors see the target workflow as workable (mentor interviews are still pending, although coordinators are also mentors) | E4, G1 |

**Who to invite:** Ms. Nina and Ms. Kelai (Operations Coordinators). If
possible, a short check with the sponsor (CSA Executive Director) on approval
and priorities, and the IT Office on platform ownership. If only one meeting
is possible, do the Operations Coordinators first and send the sponsor and IT
questions through them.

**If a meeting is not possible:** send the questions below in writing and treat
unanswered ones as `[TO CONFIRM]` in the documents. This is weaker, so say so
when submitting.

### Suggested questions

1. Looking at the four work packages (single pairing register, centralized
   mentor-change workflow, session logging, and automated matching later),
   which come first, and what is a realistic timeline before AY 2026-27
   requirements bite?
2. Who would own and operate a new platform: the unit, the IT Office, or IST?
   Is there any budget or approval needed?
3. Who approves a change to the program (for example a new school, or a change
   to the 3-session rule), and how is it communicated to coordinators and
   mentors today?
4. Does ManCom approve the mentor list? (ISS-010)
5. How would you know the program is working? Which measures would you accept,
   beyond the 3-session count?
6. What would make the unit refuse or delay a change?

## 3. Questions for Sir Pira

- Is 2026-11-27 his deadline for Assignment 4, and is it submitted through
  the G7-Repository?
- Does he expect all templates in Phases E to H, or only the necessary ones?
  Is one document per template expected?
- Where should the TOGAF Enterprise Architecture Checklist go in the repo, in
  what format, and is there a template?
- Does he expect Requirements Management as a separate deliverable?

## 4. Suggested order

1. Confirm the open questions with Sir Pira and decide F2, F3, and G2.
2. Hold the OSM meeting.
3. Build E1 to E4, then F1, G1, H1, H2 (use `/spec-driven`, Approach B suits
   documents with many unknowns).
4. Update the Roadmap and ARS, run the review, publish.

# Phase B Change List (from Phases C and D)

- **Prepared:** 2026-10-30, Clark with Laufey
- **For:** Aldrin, to apply to his own Phase B files
- **Files:** `2026-10-29 - A3 Phase B - Architecture Requirements Specification.docx` (ARS) and `2026-10-29 - A3 Phase B - Architecture Roadmap.docx` (Roadmap)
- **Source of the new content:** `2026-10-30 - A3 Phase C-D - Architecture Deliverables.docx` (section numbers below refer to that file)

Clark has not edited your files. Every item below is for you to apply, adjust, or skip.

## 1. Corrections (facts changed after Phase B)

| # | File and place | Current text | Change to | Why |
|---|---|---|---|---|
| 1 | ARS, Architecture Requirements intro, Motivation | "missing it for three consecutive semesters affects enrollment" | "two consecutive semesters" | Confirmed by Clark 2026-10-30; matches the RFAW (A1). See ISS-009 |
| 2 | ARS, Success Measures, SM-01 Baseline | "Not measured centrally; session logs are not linked to pairings" | "Confirmed sessions update OSM's master database, but pairings are split across the schools' own lists" | 2026-09-28 interview: the IT Office linked the session-log sheet to OSM's master database |
| 3 | ARS, SM-06 Baseline | "0%: the session-log sheet and the pairing lists are not connected" | "0%: session logs are tied to a typed mentor email, not to a recorded pairing" | Same as above; your point (the coordinators' lists are not linked) still holds |
| 4 | ARS, Interoperability, bullet 3 | "(today the two Google Sheets are not connected)" | "(today the schools' pairing lists are not connected to OSM's records)" | Same as above |
| 5 | ARS, Assumptions, A-05 | "The session-log sheet and the pairing lists are not connected today." | "The session-log sheet updates OSM's master database, but the schools' pairing lists are not connected to it." Status: "Interview with OSM (2026-09-28); Aldrin (2026-10-29)" | Both statements are true; this wording keeps both |
| 6 | Roadmap, 3.3 gap matrix, row "Session logs not linked to pairings" | as is | "Session logs not tied to a recorded pairing" | Same as above |
| 7 | Roadmap, 3.4 Transition Architectures | stray line "Could reference the Architecture Definition document." | delete | Leftover note |
| 8 | Roadmap, Contents page | 2.3 is listed as "Application Architecture Roadmap Components" | "Technology Architecture Roadmap Components" (right-click the contents, Update Field) | The body heading already says Technology |

## 2. Headings left for Phases C and D (fill in)

**ARS 2.3 Application Service Contracts.** Replace "To be completed in Phase C" with:

> The application services below come from the Phases C and D document (Section 3.2). Service levels are proposed and need agreement with OSM and the IT Office.

| ID | Application service | Consumer | What is provided | Proposed service level |
|---|---|---|---|---|
| S1 | Pairing Register | OSM, coordinators | Enrolled list import, mentor capacity, pairings, history across terms | Register loaded within one week of receiving the Registrar's list |
| S2 | Mentor Change Requests | Students, mentors, OSM, coordinators | One tracked queue; approved changes update the register | Within 2 working days (SM-05) |
| S3 | Session Logging | Students, mentors | Logs tied to the recorded pairing; mentor confirms by email link | Confirmation request sent to the mentor on submission |
| S4 | Compliance Monitoring and Reporting | OSM, CSA Executive Director | Session counts, early flags, semester report | Students below three sessions flagged at least 4 weeks before the semester ends; one report per semester (SM-08) |
| S5 | Notifications | All | Pairing notices, change results, reminders | Sent the same day as the triggering event |

**ARS 2.6 Implementation Standards.** Keep your business standards and add:

> Technology standards from Phase D (Section 4.2): the application runs within the university's Google Workspace where possible (TS1); UA&P sign-in for students, coordinators, and OSM, with email-link confirmation for external mentors (TS2); access by role and compliance with the Data Privacy Act of 2012 (TS3); browser access with nothing to install (TS4); one agreed Registrar list format (TS5); OSM owns the data and the IT Office maintains the tools (TS6).

**ARS 2.7 Interoperability Requirements.** After item 4 above, add a bullet:

> External mentors must be able to confirm sessions by email link without a university account.

**ARS 2.8 IT Service Management Requirements.** Replace "To be completed in Phase D" with:

> OSM owns the pairing register and refreshes it each term from the Registrar's list (graduates, transfers, new students). The IT Office maintains the application and its scripts (TS6).

**Roadmap 2.2 Information Systems Roadmap Components.** Replace the placeholder with:

| ID | Candidate component | Gap it closes | Supports |
|---|---|---|---|
| IS-01 | Pairing Register (S1), with Pairing and Mentor Capacity records | Schools' lists not linked to OSM; pairings not kept | BA-01, BA-02, BA-03, BA-05 |
| IS-02 | Mentor Change Requests (S2) | Changes handled only by email | BA-04 |
| IS-03 | Session logs tied to the recorded pairing (S3) | Logs tied to a typed mentor email | BA-06 |
| IS-04 | Compliance Monitoring and Reporting (S4) | No early warning; no formal report | BA-06, BA-07 |
| IS-05 | Notifications (S5) | Notices sent as separate emails | BA-03, BA-04 |

**Roadmap 2.3 Technology Roadmap Components.** Replace the placeholder with:

| ID | Candidate component | Gap it closes | Supports |
|---|---|---|---|
| TA-01 | Access by role on the shared data (TS3) | Several people can edit the shared sheets | BA-01, BA-06 |
| TA-02 | One agreed Registrar list format (TS5) | No agreed format for the list | BA-02 |
| TA-03 | Support split: OSM owns the data, the IT Office maintains the tools (TS6) | No named owner for upkeep | BA-01 |

**Roadmap 3.3 gap matrix.** Add these rows below the Business rows:

| Architecture domain | Gap | Potential solutions | Dependencies |
|---|---|---|---|
| Data | Session logs not tied to a recorded pairing | Session Log linked to Pairing (IS-03) | IS-01 |
| Data | Mentor changes and capacity kept only in email | Change Request and Capacity records (IS-01, IS-02) | IS-01 |
| Application | Coordinator lists and email chains | Pairing Register, Change Requests, Notifications (IS-01, IS-02, IS-05) | Coordinator adoption (A-03) |
| Application | No early warning on session counts | Compliance Monitoring (IS-04) | IS-03 |
| Technology | Shared sheets editable by several people | Access by role (TA-01) | IT Office support (A-06) |
| Technology | No agreed Registrar list format | One format each term (TA-02) | Registrar agreement (A-02) |

**Roadmap 3.4 Transition Architectures.** Add the new IDs to the two transitions:

- Transition 1: add IS-01, IS-02, TA-01, TA-02, TA-03.
- Transition 2: add IS-03, IS-04, IS-05.

## 3. Phase E headings (recommendation only)

ARS 2.5, Roadmap 3.1, 3.2, and 3.5 are Phase E work, which is outside A3 (Phases A to D). Recommendation: keep each heading but replace its body with one line:

> Developed in Phase E (Opportunities and Solutions), which is outside the scope of this assignment (Phases A to D).

This shows the team knows where each section belongs, without leaving it looking empty. Your call.

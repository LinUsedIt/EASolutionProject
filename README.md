# EASolutionProject

> **Course:** IT Elective: Solution Architecture. Despite the name, this
> course is about **Enterprise Architecture (EA)**, and that's the lens for
> all the work in this repo.
> **Professor:** Sir Pira
> **Team:** Emmanuel Velasco · Deejay Clark Datu · Aldrin
> **Status:** In progress

## 1. Project Description

This repository is the team's working space for an Enterprise Architecture
practicum built around the TOGAF® Standard. The team applies the TOGAF
Architecture Development Method (ADM) to a real enterprise: the
**Mentoring Unit of the Center for Student Affairs (CSA), University of
Asia and the Pacific (UA&P)**. The team interviewed its operations
coordinators on 2026-09-11 and 2026-09-28.

There are no fixed roles or deliverables. The team works on whatever the
professor asks for. Each request is recorded in
[`AI Directory/Assignments.md`](AI%20Directory/Assignments.md) so nothing
gets lost between sessions.

## 2. Working with Laufey (the AI assistant)

Laufey is Claude Code, set up for this project by
[`CLAUDE.md`](CLAUDE.md) and the files in `.claude/`.

**Always open Claude Code from the `EASolutionProject` folder.** That's
how it finds Laufey's rules, memory, skills, and settings. Opened from
any other folder, it's just plain Claude.

Useful commands (Laufey also uses these on its own when your request
matches):

| Command | What it does |
|---|---|
| `/analyze-document` | Reviews a draft or document against TOGAF and the professor's requirements |
| `/summarize-document` | Gives a faithful summary of a document |
| `/plan-work` | Makes a plan with tasks, owners, and dates, or stress-tests yours |
| `/make-study-guide` | Writes a chapter study guide into `Course Files/Study Guides/` |
| `/log-assignment` | Records what the professor asked for |
| `/log-issue` | Adds, updates, or closes an issue |
| `/log-session` | Records the session in the memory files |

Laufey asks what format you want (Markdown, Word, or PDF) before creating
a file, unless you've already said.

## 3. How the Repo Is Organized

The repo is organized around **who uses each part**.

| Path | What's there |
|---|---|
| [`CLAUDE.md`](CLAUDE.md) | Laufey's identity, personality, and project context. Loads every session. |
| `.claude/rules/` | Laufey's detailed rules, one topic per file. Load every session. |
| `.claude/skills/` | The slash commands above |
| `.claude/agents/` | Two helper agents: `togaf-researcher` (finds cited passages in the Readings) and `deliverable-reviewer` (independent review of drafts) |
| `.claude/settings.json` | Makes Claude Code ask before Laufey edits its own rules or the team's files |
| **AI Directory/** | Laufey's memory and outputs |
| [`MemoryBank.md`](AI%20Directory/MemoryBank.md) | Current project snapshot, decisions, open questions |
| [`Assignments.md`](AI%20Directory/Assignments.md) | Everything the professor has asked for |
| [`SessionLog.md`](AI%20Directory/SessionLog.md) | History of every session, newest first |
| `Generated Outputs/` | Analyses, plans, summaries, and drafts Laufey produces |
| `Workflows/` | Replaced by the skills in `.claude/skills/` |
| **Course Files/** | Shared course material |
| `Readings/` | The only TOGAF sources Laufey cites: The TOGAF® Standard 10th Ed., the TOGAF® EA Foundation Study Guide, and *Mastering the TOGAF® Standard* (Eric Jager) |
| `Study Guides/` | Chapter study guides |
| `AI Explanations/` | Concept explanations Laufey writes on request |
| `TOGAF Templates/` | Official deliverable templates, one folder per ADM phase |
| **Users Directory/** | The team's own work |
| `Course Assignments/` | Drafts, notes, interviews, and submissions, one folder per assignment |
| `Issues/` | [`CurrentIssues.md`](Users%20Directory/Issues/CurrentIssues.md) and `CurrentIssuesList.csv`, kept in sync |

> **Note:** the professor's assignment guides are instructions for the
> assignment, not TOGAF sources. Laufey uses them for requirements only.

## 4. Changing Laufey's Rules

Edit `CLAUDE.md` or the files in `.claude/rules/` directly, or ask Laufey
to propose a change. It won't edit them without your approval. Keep
rules short and specific: Claude follows concise instructions more
reliably than long ones.

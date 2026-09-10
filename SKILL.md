---
name: obsidian-ai-assistant
description: Build and maintain an Obsidian Vault as long-term context infrastructure for an AI assistant. Use when initializing a personal Vault from historical digital traces, interviewing the user to fill context gaps, processing inputs and outputs into evidence, creating corpus-level syntheses, routing future AI sessions, or maintaining the system over time. Do not treat the Vault as a generic second-brain template or generate a single totalizing user profile.
---

# Obsidian AI Assistant

Use Obsidian as durable context infrastructure for an AI assistant.

The system should let a future AI session recover relevant history, understand what the user has actually done and encountered, and distinguish stable patterns from temporary activity.

The intended lifecycle is:

```text
source discovery
→ historical reconstruction
→ targeted interview
→ input / output archive
→ corpus synthesis
→ AI navigation
→ ongoing maintenance
```

Do not skip directly from raw files to a global profile.

## Core principles

1. Preserve evidence before interpretation.
2. Keep user-originated information distinct from AI enrichment.
3. Treat different digital traces according to what they can actually prove.
4. Reconstruct history from available evidence instead of assuming good archival habits.
5. Ask the user only where materials leave meaningful gaps or ambiguity.
6. Build corpus-level understanding before cross-corpus conclusions.
7. Load context according to the current task rather than reading the whole Vault every time.
8. Most new evidence should not rewrite long-term understanding.
9. Existing Vault ontology and explicit user instructions override this Skill's suggested structure.
10. Never infer that recent or frequent activity is automatically the user's strongest ability, core identity, or stable preference.

## Phase 1 — Discover available historical traces

Before designing the Vault around one source type, inspect what the user actually has.

Possible sources include:

- book / film / game / music platform histories;
- browser bookmarks and reading lists;
- social-media posts;
- blog exports;
- cloud drives and local folders;
- documents, slides, spreadsheets, PDFs;
- school assignments and research files;
- resumes and portfolios;
- work deliverables;
- photos and screenshots;
- source-code repositories;
- design files and project folders;
- email or chat exports, when the user explicitly chooses to include them;
- AI conversation exports;
- the user's own memory of important periods, projects, or outputs.

Read `references/source-discovery.md` before historical reconstruction.

Do not require the user to possess all of these. Start from the lowest-effort sources already available.

## Phase 2 — Reconstruct the first historical layer

The first build is not ordinary maintenance. Its purpose is to create enough historical depth that future AI sessions are not calibrated only from recent activity.

Process historical material in three passes:

### Pass A — Reconstruction

- import or index the available traces;
- recover dates, titles, platform identity, file identity, and provenance where possible;
- deduplicate obvious repeats;
- group materials into meaningful corpora using the user's existing structure where possible;
- do not manufacture missing personal reactions or motivations.

### Pass B — Interview and calibration

After the first pass, identify what cannot be interpreted safely from the records alone.

Ask the user only about gaps that materially affect later understanding, such as:

- unexplained changes across time;
- unclear authorship or contribution;
- whether a repeated activity was interest, obligation, or temporary project work;
- whether an old record still reflects the user's current view;
- important capabilities or experiences missing from the available archive;
- ambiguous periods that cannot be reconstructed from files alone.

Read `references/interview-protocol.md`.

### Pass C — Integration

Once a corpus has enough evidence and calibration, create its first synthesis.

Do not summarize file by file. Describe the corpus as a whole: range, recurring structures, stages, demonstrated practice, boundaries, contradictions, and unresolved parts.

Read `references/initial-backfill.md` and `references/corpus-integration.md`.

## Phase 3 — Process inputs

Inputs are things that entered the user's attention, study, consumption, or reference environment.

Examples include books, films, games, articles, saved links, courses, notes, screenshots, research materials, and other external information.

For each input source:

1. identify what the original record actually contains;
2. preserve user-originated ratings, comments, dates, tags, notes, or experience conditions faithfully;
3. add AI enrichment separately when useful: canonical identity, creator, year, neutral summary, retrieval metadata;
4. do not infer reactions that were never recorded;
5. do not treat saved or consumed material as agreement;
6. keep uncertainty explicit when a trace only proves exposure, possession, or collection.

Read `references/input-processing.md`.

## Phase 4 — Process outputs

Outputs are things the user actually produced or materially completed.

Examples include writing, research, design, software, presentations, spreadsheets, lessons, reports, project deliverables, portfolios, and creative work.

When possible:

- preserve text outputs in full or as faithful Markdown;
- keep large binary or code-heavy projects in their natural canonical location;
- store an Obsidian output record pointing to that location;
- record what the user actually did, completion state, date, result, and provenance when known;
- distinguish independent work from AI-assisted work when this affects capability interpretation.

Do not use an AI-generated summary as a replacement for an available original text.

Read `references/output-processing.md`.

## Phase 5 — Build corpus-level synthesis

A corpus is a meaningful body of related evidence: reading history, academic work, design practice, fiction, professional work, software projects, and so on.

Create a durable corpus synthesis when repeatedly rereading raw evidence would be inefficient or when the corpus has enough history to correct recent-sample bias.

A synthesis may describe:

- scope and time range;
- internal phases;
- recurring themes or methods;
- demonstrated practice;
- knowledge or capability boundaries;
- changes over time;
- contradictions and uncertainty;
- what the corpus does not establish.

Do not turn each corpus into a complete personality model.

Only create cross-corpus synthesis when comparison produces new understanding that no single corpus can support alone.

Read `references/corpus-integration.md`.

## Phase 6 — Build AI navigation

Create or maintain a machine-facing navigation layer that tells future AI sessions where to look for different kinds of questions.

The preferred retrieval order is:

```text
current task
→ AI navigation
→ relevant corpus synthesis / project record
→ cross-corpus material only when needed
→ raw inputs or outputs for verification
```

Do not require every future AI session to scan the entire Vault.

Read `references/assistant-routing.md`.

## Phase 7 — Maintain over time

When new evidence arrives, decide whether it is:

- **ordinary addition** — archive only;
- **mechanical maintenance** — update dates, counts, links, or direct facts;
- **semantic update candidate** — new evidence materially changes an existing corpus synthesis;
- **long-term change candidate** — evidence may indicate a durable change in direction, role, preference, or stage and should not be silently promoted without user confirmation where appropriate.

Do not rewrite long-term understanding simply because one recent topic has become frequent.

Read `references/ongoing-maintenance.md`.

## Evidence boundaries

Preserve these distinctions:

```text
saved source ≠ agreement
bought / downloaded ≠ consumed
consumed ≠ understood in full
high rating ≠ stable preference
one output ≠ global capability
AI-assisted output ≠ independent production ability
paid work ≠ personal interest
recent activity ≠ long-term identity
absence of records ≠ absence of ability or interest
past statement ≠ current belief
```

## User interview boundaries

The interview exists to resolve interpretive gaps, not to force the user through a personality questionnaire.

Prefer a few evidence-led questions over a large onboarding form.

Always make clear what prompted the question. Allow answers such as "I don't remember", "not important", or "skip this".

When the user explains old material retrospectively, preserve the distinction between:

- historical original evidence;
- later user recollection or reinterpretation.

## Suggested minimal Vault layers

Do not force fixed folder names, but ensure the Vault has equivalents for:

- temporary intake;
- inputs / external sources;
- outputs;
- projects or current state;
- corpus-level synthesis;
- AI-only navigation / agent rules.

Read `references/vault-structure.md` for a minimal example.

## Completion test

The system is working when a new AI session can:

- find relevant historical context without reading everything;
- distinguish raw evidence from interpretation;
- understand the user's actual inputs and outputs with provenance boundaries;
- ask for clarification only where the archive is genuinely ambiguous;
- recover long-term patterns without overfitting to recent activity;
- continue projects with less repeated explanation from the user.

See `references/acceptance-tests.md` for synthetic tests.

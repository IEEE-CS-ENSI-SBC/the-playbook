# Resource Repo Scaffold Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Stand up the initial category tree, navigation, review ledger, and
contribution rubric for `the-playbook`, so resource review can start.

**Architecture:** Plain markdown, no build step. Four top-level category
folders (`devsecops`, `gamedev`, `cyber`, `general`), each with a
`README.md` (breadcrumb to Home + "no resources yet" placeholder). Home
`README.md` keeps its existing intro and gains a links table. Two root
files, `REVIEW_LOG.md` and `CONTRIBUTING.md`, carry the audit trail and
the rubric respectively.

**Tech Stack:** Markdown only.

**Spec:** `docs/superpowers/specs/2026-11-12-resource-repo-structure-design.md`

## Global Constraints

- Folder names: lowercase kebab-case.
- Resource line format (for future use, documented now): `- **[Title](url)** — one-line description of why it's useful.`
- New sub-category only once a category's README would exceed ~15 resources, or 3+ clearly distinct clusters appear — no speculative empty subfolders.
- Resources are only ever added via the user+assistant chat review flow — no external contributor path, so `CONTRIBUTING.md` carries no PR/issue submission mechanics.
- `docs/superpowers/specs/` stays committed but is not linked from the Home README.
- Home `README.md`'s existing one-line chapter description is kept verbatim; links are added below it, not a rewrite.
- `REVIEW_LOG.md` category column for a rejected resource names what it was considered for, clearly marked as not an actual placement.

## Review Focus

- A category folder with no resources yet must still render cleanly on GitHub (not a broken/empty list) — placeholder text, not an empty bullet.
- Home README's category table must link to real files (`devsecops/README.md` etc.), not guessed paths — a typo'd relative link silently 404s on GitHub with no local error.
- `CONTRIBUTING.md`'s rubric and taxonomy rules must match the spec's wording exactly (four-point rubric, split threshold, naming convention) — paraphrasing here is how the spec and the shipped file drift apart over time.
- `REVIEW_LOG.md`'s header must make the "category assigned" column's reject-case semantics explicit inline, not just rely on this plan/spec being read later.
- Every new file needs a parent-relative breadcrumb link back to Home that actually resolves (`../README.md` from inside a category folder), since broken breadcrumbs defeat the whole "jump back up" navigation goal.

---

## Task 1: Category folder scaffolding

**Files:**
- Create: `devsecops/README.md`
- Create: `gamedev/README.md`
- Create: `cyber/README.md`
- Create: `general/README.md`

**Interfaces:**
- Produces: four category README files, each with a `[← Home](../README.md)` breadcrumb line, a top-level `# <Category>` heading, and a `_No resources yet — check back soon._` placeholder line where resources will later be listed.

- [ ] **Step 1: Write `devsecops/README.md`**

Content:
```markdown
[← Home](../README.md)

# DevSecOps

Secure coding and deployment practices tied directly to application and
software development: secure coding, CI/CD pipeline security, dependency
and supply-chain scanning, container and deployment security, git
security, and related tooling.

_No resources yet — check back soon._
```

- [ ] **Step 2: Write `gamedev/README.md`**

Content:
```markdown
[← Home](../README.md)

# Game Dev

Game engines, game design, game programming, and game art/audio/tooling.

_No resources yet — check back soon._
```

- [ ] **Step 3: Write `cyber/README.md`**

Content:
```markdown
[← Home](../README.md)

# Cyber

Security topics not tied directly to the software development lifecycle:
offensive security/pentesting, CTF, network security, firmware, reverse
engineering, forensics, malware analysis, cryptography.

_No resources yet — check back soon._
```

- [ ] **Step 4: Write `general/README.md`**

Content:
```markdown
[← Home](../README.md)

# General

Cross-field CS fundamentals, programming languages, dev tools and
productivity, career/soft-skills — anything not specific to one of the
other fields.

_No resources yet — check back soon._
```

- [ ] **Step 5: Verify all four files render the breadcrumb and heading**

Run: `for f in devsecops gamedev cyber general; do echo "--$f--"; cat "$f/README.md"; done`
Expected: each prints its breadcrumb line, heading, description, and placeholder line with no errors.

- [ ] **Step 6: Commit**

```bash
git add devsecops/README.md gamedev/README.md cyber/README.md general/README.md
git commit -m "Scaffold top-level category folders"
```

---

## Task 2: Home README navigation

**Files:**
- Modify: `README.md`

**Interfaces:**
- Consumes: the four category README paths produced by Task 1 (`devsecops/README.md`, `gamedev/README.md`, `cyber/README.md`, `general/README.md`).

- [ ] **Step 1: Append a categories section below the existing intro line**

Keep the existing line (`IEEE ENSI SB CS Chapter's playbook: ...`) exactly
as-is, then add:
```markdown

## Categories

- [DevSecOps](devsecops/README.md) — secure coding & deployment
- [Game Dev](gamedev/README.md) — engines, design, programming, art
- [Cyber](cyber/README.md) — offensive security, CTF, reverse engineering, and more
- [General](general/README.md) — CS fundamentals, tools, career
```

- [ ] **Step 2: Verify links resolve to real files**

Run: `grep -oP '\]\(\K[^)]+' README.md | xargs -I{} test -f {} && echo OK`
Expected: `OK` printed once per link, no "No such file" errors.

- [ ] **Step 3: Commit**

```bash
git add README.md
git commit -m "Add category navigation to home README"
```

---

## Task 3: Review ledger

**Files:**
- Create: `REVIEW_LOG.md`

**Interfaces:**
- Produces: the append-only review audit trail later review turns write one line into per resource.

- [ ] **Step 1: Write `REVIEW_LOG.md`**

Content:
```markdown
# Review Log

Append-only record of every resource review decision. Not linked from the
Home README — this is for maintainers, not workshop browsing.

Columns:
- **Date** — YYYY-MM-DD
- **Resource** — `[Title](url)`
- **Category** — where it was filed if kept; if rejected, the category it
  was considered for, written as `considered: <category> — rejected`
- **Verdict** — `kept` or `rejected`
- **Rationale** — one line, why

| Date | Resource | Category | Verdict | Rationale |
|------|----------|----------|---------|-----------|
```

- [ ] **Step 2: Verify the file parses as a table**

Run: `cat REVIEW_LOG.md`
Expected: header row and separator row present, zero data rows, no syntax errors.

- [ ] **Step 3: Commit**

```bash
git add REVIEW_LOG.md
git commit -m "Add review log for resource decisions"
```

---

## Task 4: Contribution rubric

**Files:**
- Create: `CONTRIBUTING.md`

**Interfaces:**
- Produces: the rubric and taxonomy rules future review turns (and future sessions) apply.

- [ ] **Step 1: Write `CONTRIBUTING.md`**

Content:
```markdown
# Contributing

Resources are added through a review conversation between the chapter
exec and the assistant — there is currently no external PR/issue path.
This file exists so that rubric and taxonomy stay consistent across
sessions.

## Acceptance rubric

A resource is kept only if it is:

1. **Credible / accurate.**
2. **Genuinely useful** for the field or sub-category it would sit in.
3. **Not redundant** with an existing resource that covers the same
   ground equally well or better.
4. **Reasonably durable** — unlikely to vanish or paywall soon. Prefer
   free resources over paid when quality is comparable.

## Taxonomy rules

- Folder names: lowercase kebab-case (e.g. `reverse-engineering`, not
  `reverse_eng`).
- A new sub-category is only created once a category's README would
  otherwise exceed roughly 15 resources, or once 3+ clearly distinct
  clusters show up in it. Don't pre-create empty subfolders.
- Every category/sub-category folder has its own `README.md`: a
  breadcrumb link up, links down to any sub-categories, then its own
  resources.
- Resource line format: `- **[Title](url)** — one-line description of
  why it's useful.`
- `devsecops` = secure coding/deployment tied directly to the SDLC (git
  security, CI/CD, dependency/supply-chain scanning, container &
  deployment security). `cyber` = security topics not tied directly to
  the SDLC (offensive security, CTF, network security, firmware,
  reverse engineering, forensics, malware analysis, cryptography).
```

- [ ] **Step 2: Verify the file exists and the rubric/taxonomy sections are both present**

Run: `grep -c '^## ' CONTRIBUTING.md`
Expected: `2`

- [ ] **Step 3: Commit**

```bash
git add CONTRIBUTING.md
git commit -m "Add contribution rubric and taxonomy rules"
```

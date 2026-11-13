# The Playbook — resource repo structure & review process

## Intent / why

`the-playbook` is IEEE ENSI SB CS Chapter's living collection of vetted
resources (guides, cheatsheets, tools, courses) used to prep and run
workshops across several fields. Today it's a one-line README and
nothing else. Resources will arrive one at a time (pasted links), get
reviewed jointly, and — if kept — filed into a category tree that stays
coherent as it grows. The repo needs to serve two audiences at once:
chapter members skimming for a specific workshop topic, and whoever
(often a future session of this same assistant) does the next review and
needs to know what's already been decided and why.

## Goals

- A category tree that starts at `devsecops`, `gamedev`, `cyber`,
  `general` and can grow new top-level fields later without a rewrite.
- Every accepted resource lives in the most specific category/sub-category
  that fits, with a one-line description.
- Anyone can navigate from the home README down to any resource, and
  jump back up, without ever facing a huge flat list.
- Every review decision (kept or rejected) is recorded with a reason, so
  it isn't re-litigated later and so category drift is visible over time.
- The taxonomy itself is revisited at each review — categories can be
  split, merged, or renamed as the collection grows, not frozen on day one.

## Non-goals

- No build step / static site generator / index-generation script. Plain
  GitHub-rendered markdown only.
- No automated resource discovery or link-checking automation (can be a
  later ask, not now).
- No multi-language content.

## Anti-goals (would make this a failure even if "technically done")

- A category README that grows into an unreadable wall of links.
- Folder sprawl: many near-empty sub-categories created pre-emptively.
- A resource re-reviewed (or re-rejected) because nobody could tell it
  had already been decided on.
- `devsecops` and `cyber` entries that overlap/duplicate because the
  boundary wasn't applied consistently.

## Constraints

- Markdown only, rendered by GitHub — no tooling dependency.
- Review is interactive and incremental: the user pastes one resource at
  a time; review decisions are joint (I propose category + keep/reject
  rationale, the user confirms or overrides).
- Audience includes less-technical chapter members — navigation must stay
  shallow and obvious, not just "technically browsable."

## Approaches considered

- **A — Nested READMEs only.** Simplest; no persistent rationale for past
  decisions, so every future session re-derives context from scratch.
- **B — Nested READMEs + a root `REVIEW_LOG.md` ledger.** Same browsing
  tree as A, plus one append-only log of every review decision (resource,
  category, verdict, date, rationale). Minimal overhead, real memory.
- **C — B plus per-resource metadata files rendered into READMEs by a
  script.** Most powerful, but needs a build step — overkill here and
  works against the "don't overwhelm" goal.

**Picked: B** (user confirmed).

## Decided

- **Top-level categories (for now):** `devsecops`, `gamedev`, `cyber`,
  `general`. More can be added later as siblings.
- **`devsecops` scope (user-defined):** secure coding and deployment
  practices tied directly to application/software development — e.g.
  git security, dependency/supply-chain scanning, CI/CD pipeline
  security, container & deployment security, SAST/DAST-in-the-pipeline.
- **`cyber` scope (user-defined, by elimination):** security topics not
  tied directly to the SDLC — offensive security/pentesting, CTF,
  network security, firmware, reverse engineering, forensics, malware
  analysis, cryptography.
- **`gamedev` scope (my call):** engines (Unity/Unreal/Godot/other),
  game design, game programming, game art/audio/tooling.
- **`general` scope (my call):** cross-field CS fundamentals,
  programming languages, dev tools/productivity, career/soft-skills —
  the catch-all for anything not specific to one of the other fields.
- **Folder naming:** lowercase kebab-case (e.g. `reverse-engineering`,
  not `reverse_eng`).
- **Sub-categorization depth:** as deep as needed (the user's own example
  was `devsecops/git`, `cyber/firmware/reverse-engineering`), but a new
  sub-category is only created once a category's README would otherwise
  exceed roughly 15 resources, or once 3+ clearly distinct clusters show
  up in it. Don't pre-create empty subfolders speculatively.
- **Resource line format:** `- **[Title](url)** — one-line description of
  why it's useful.` Tags are optional and only added if they're pulling
  real weight (e.g. `_(free)_`, `_(video)_`) — no mandatory tag schema.
- **Every category/sub-category folder has a `README.md`** containing:
  a one-line breadcrumb/back-link to its parent (or Home), a bullet list
  of links down to its own sub-categories (if any), then its own
  resources.
- **Home `README.md`** gets a short intro plus a table/list linking to
  each top-level category.
- **`REVIEW_LOG.md`** at repo root, append-only, one line per reviewed
  resource: date, title+link, category assigned, verdict (kept/rejected),
  one-line rationale. This is the maintainers' audit trail, not meant for
  workshop-goer browsing.
- **`CONTRIBUTING.md`** at repo root documents the review rubric so
  future chapter members (and future sessions) apply it consistently.
  Proposed default rubric (my call, open to the user tuning it over
  time): the resource must be (1) credible/accurate, (2) genuinely useful
  for the field/sub-category it'd sit in, (3) not redundant with an
  existing resource covering the same ground equally well or better,
  (4) reasonably durable (not likely to vanish/paywall soon), with free
  resources preferred over paid when quality is comparable. It also
  states the folder-naming convention and the sub-category split
  threshold from this doc, so a future session without this spec can
  still keep the tree consistent. Resources are only ever added through
  the user + assistant chat review flow (confirmed) — no outside
  contributor path, so the file does not need PR/issue submission
  mechanics.
- **`docs/superpowers/specs/`** (this planning doc) stays committed for
  history, but isn't linked from the Home README — it's internal process
  documentation, not something a workshop-goer browsing resources needs
  to find.
- **Home `README.md`** keeps the chapter's existing one-line description
  verbatim; the category links are added below it, not a rewrite.
- **`REVIEW_LOG.md`**'s category column, for a rejected resource, names
  the category it was being considered for, clearly marked as not an
  actual placement (e.g. "considered: cyber/network — rejected").
- **Review flow going forward:** user pastes a resource → I check it
  against the rubric, propose a category (creating a new sub-category
  only if the threshold above is crossed) and a keep/reject call with a
  one-line reason → user confirms or overrides → I add the entry (if
  kept) to the right README and always append a line to
  `REVIEW_LOG.md`, and reshuffle the tree if the addition reveals the
  taxonomy no longer fits.

## Left to the builder (initial scaffold)

- Create the four top-level category folders, each with a `README.md`
  (breadcrumb to Home, "no resources yet").
- Update the Home `README.md` with the intro + links to the four
  category READMEs.
- Create `REVIEW_LOG.md` with a header row/format explanation and no
  entries yet.
- Create `CONTRIBUTING.md` with the rubric above.
- No resources are added in the scaffold — that starts once the user
  pastes the first one.

# Contributing

Resources are added through a review conversation between the chapter
exec and the assistant — there is currently no external PR/issue path.
This file exists so that rubric and taxonomy stay consistent across
sessions.

## Acceptance rubric

A resource is kept only if it is credible/accurate and reasonably
durable (unlikely to vanish or paywall soon — prefer free over paid when
quality is comparable), **and** it clears this bar:

1. **Fundamental / genuinely useful** — it teaches or covers something
   core to the field, not a minor variant of something already covered.
   File it by what it's PRIMARILY about, not every field it's useful
   for — e.g. a general C++ channel that happens to have one game-engine
   series stays in `general/languages`, not `game-dev`; a channel whose
   whole identity is building games from scratch belongs in `game-dev`
   even though it uses a general-purpose language to do it.
2. **Good enough on its own merits** — if it's credible and genuinely
   useful, add it. Overlap with an existing resource is not a reason to
   skip a good one; only skip a *weak or thin* duplicate that adds
   nothing and would just be clutter.
3. **Truly necessary** — would the category have a real gap without it,
   or is it fine as-is?
4. **Doesn't overwhelm** — would adding it clutter the list more than
   its unique value earns? A lean list of resources that each pull real
   weight beats exhaustive coverage. When in doubt and it adds nothing
   unique, leave it out.

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
- Books: never link to a pirated/unauthorized copy. If there's no
  official source (publisher page, author's site, legitimate preview),
  list it unlinked as `- **Title** — Author — one-line description.`
  rather than skipping it.
- Within a list, order resources by how fundamental/necessary they are —
  the one you'd point someone to first goes first, situational or
  deep-dive resources go later.
- `devsecops` = secure coding/deployment tied directly to the SDLC (git
  security, CI/CD, dependency/supply-chain scanning, container &
  deployment security). `cyber` = security topics not tied directly to
  the SDLC (offensive security, CTF, network security, firmware,
  reverse engineering, forensics, malware analysis, cryptography).
  `software-dev` = application-level programming and design only (web,
  mobile, desktop apps). `computer-science` = theory and fundamentals
  (algorithms, program design, computability) — not hands-on hardware or
  networking. `systems` = the applied/hands-on side of how computers
  work (computer architecture, OS, networking internals, low-level
  programming). `general` = tools, references, productivity, career —
  the catch-all for what doesn't fit the above.

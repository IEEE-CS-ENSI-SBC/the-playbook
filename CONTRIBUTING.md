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
2. **Adds something unique** — what does it offer that nothing else
   already in that category/sub-category covers? If an existing
   resource covers the same ground equally well, skip the new one, even
   if it's good.
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
- Within a list, order resources by how fundamental/necessary they are —
  the one you'd point someone to first goes first, situational or
  deep-dive resources go later.
- `devsecops` = secure coding/deployment tied directly to the SDLC (git
  security, CI/CD, dependency/supply-chain scanning, container &
  deployment security). `cyber` = security topics not tied directly to
  the SDLC (offensive security, CTF, network security, firmware,
  reverse engineering, forensics, malware analysis, cryptography).

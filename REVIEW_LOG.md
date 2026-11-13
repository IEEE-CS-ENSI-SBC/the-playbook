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
| 2026-11-12 | [roadmap.sh](https://roadmap.sh/) | general | kept | Foundational "where do I start" resource spanning fields; nothing else fills that role; doesn't overlap or clutter. |
| 2026-11-12 | [linuxcommand.org](https://linuxcommand.org/) | general | kept | Canonical ground-up shell/bash tutorial; foundational across fields; distinct from roadmap.sh, no overlap. |
| 2026-11-12 | [OverTheWire: Bandit](https://overthewire.org/wargames/bandit/) | cyber | kept | Classic beginner CTF/wargame; hands-on practice, distinct from reading-material resources; standard starting point for cyber intros. |
| 2026-11-12 | [ShellCheck](https://www.shellcheck.net/) | devsecops | kept | Secure-coding tool for shell scripts, directly relevant to CI/CD pipelines; first devsecops entry, distinct type (tool, not tutorial). |
| 2026-11-12 | [Atlassian Git Tutorials](https://www.atlassian.com/git/tutorials) | devsecops/git | kept | Fundamental git reference; fills a real gap; created devsecops/git subcategory as previously flagged by user's own example. |
| 2026-11-12 | [Learn Git Branching](https://learngitbranching.js.org/) | devsecops/git | kept | Interactive visual branching sandbox; distinct type (practice vs reference) from Atlassian tutorials. |
| 2026-11-12 | [Git Immersion](https://gitimmersion.com/) | considered: devsecops/git — rejected | rejected | Third "learn git from scratch" resource; overlaps with Atlassian tutorials + Learn Git Branching without a distinct enough angle. |
| 2026-11-12 | [Oh Shit, Git!?!](https://ohshitgit.com/) | devsecops/git | kept | Distinct angle: fixing mistakes, not learning fundamentals; real recurring need nothing else here covers. |
| 2026-11-12 | [Pro Git](https://git-scm.com/book/en/v2) | devsecops/git | kept | Official authoritative deep reference, distinct tier from Atlassian's practical tutorial. |
| 2026-11-12 | [Docker: Get Started](https://docs.docker.com/get-started/) | devsecops/docker | kept | Official canonical getting-started guide; created devsecops/docker subcategory. User chose to keep alongside 101-tutorial despite likely overlap. |
| 2026-11-12 | [Docker 101 Tutorial](https://www.docker.com/101-tutorial/) | devsecops/docker | kept | Official interactive beginner track; flagged as possibly overlapping with Get Started, user chose to keep both. |
| 2026-11-12 | [Docker Curriculum](https://docker-curriculum.com/) | devsecops/docker | kept | Community tutorial with distinct end-to-end deployment angle. |

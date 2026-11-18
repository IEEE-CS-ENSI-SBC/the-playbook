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
| 2026-11-18 | [Kubernetes Basics](https://kubernetes.io/docs/tutorials/kubernetes-basics/) | devsecops/kubernetes | kept | Official interactive tutorial; created devsecops/kubernetes subcategory. |
| 2026-11-18 | [Introduction to Kubernetes (LFS158x)](https://training.linuxfoundation.org/training/introduction-to-kubernetes/) | devsecops/kubernetes | kept | Broader structured course (architecture/networking/security), distinct depth from the quick tutorial. |
| 2026-11-18 | [Semgrep Academy: Secure Coding](https://academy.semgrep.dev/courses/secure-coding) | devsecops | kept | First secure-coding-practices resource; fills a real gap beyond ShellCheck's narrow linting scope. |
| 2026-11-18 | [Professor Messer](https://www.professormesser.com/) | cyber | kept | Free CompTIA (Security+/Network+) video courses; theory foundation distinct from Bandit's hands-on wargame. |
| 2026-11-18 | [Awesome Selfhosted](https://github.com/awesome-selfhosted/awesome-selfhosted) | considered: devsecops — rejected | rejected | Software catalog, not a learning resource; doesn't teach a skill tied to any of the four fields. |
| 2026-11-18 | [Kubernetes the Hard Way](https://github.com/kelseyhightower/kubernetes-the-hard-way) | devsecops/kubernetes | kept | Manual-bootstrap internals deep-dive, distinct from the quickstart tutorial and the structured course already filed. |
| 2026-11-18 | [90DaysOfDevOps](https://github.com/MichaelCade/90DaysOfDevOps) | devsecops | kept | Comprehensive cross-topic curriculum tying the whole domain together; distinct role from single-topic subcategories. |
| 2026-11-18 | [DevOps Exercises](https://github.com/bregman-arie/devops-exercises) | devsecops | kept | Self-test/interview-prep question bank; distinct purpose from curriculum/tutorial resources already filed. |
| 2026-11-18 | [Terraform Tutorials](https://developer.hashicorp.com/terraform/tutorials) | devsecops/terraform | kept | First IaC/Terraform resource; created devsecops/terraform subcategory. |
| 2026-11-18 | [Prometheus: Overview](https://prometheus.io/docs/introduction/overview/) | devsecops/monitoring | kept | First observability/monitoring resource; created devsecops/monitoring subcategory (named by topic, not tool, for future additions like Grafana). |
| 2026-11-18 | [Kubernetes Docs](https://kubernetes.io/docs/home/) | devsecops/kubernetes | kept | Full reference manual, distinct role (ongoing reference) from tutorial/course/hard-way already filed. |
| 2026-11-18 | [Helm Docs](https://helm.sh/docs/) | devsecops/kubernetes | kept | K8s package manager; tightly coupled to the kubernetes ecosystem rather than a standalone pillar, so filed inside the subcategory, not a new one. |
| 2026-11-18 | [Grafana Tutorials](https://grafana.com/tutorials/) | devsecops/monitoring | kept | Visualization layer complementing Prometheus's metrics collection; completes the standard observability stack. |
| 2026-11-18 | [GitLab CI/CD Docs](https://docs.gitlab.com/ci/) | devsecops/ci-cd | kept | First dedicated CI/CD resource; created devsecops/ci-cd subcategory — central to the category's own definition. |
| 2026-11-18 | [GitHub Actions Docs](https://docs.github.com/en/actions) | devsecops/ci-cd | kept | Different major CI/CD platform (GitHub vs GitLab); distinct syntax/ecosystem, not a duplicate. |
| 2026-11-18 | [Docker Docs](https://docs.docker.com/) | devsecops/docker | kept | Full reference manual, distinct role (ongoing reference) from the get-started tutorial, same pattern as Kubernetes Docs. |
| 2026-11-18 | [Ansible: Getting Started](https://docs.ansible.com/projects/ansible/latest/getting_started/index.html) | devsecops/ansible | kept | First config-management resource; created devsecops/ansible subcategory — complements Terraform's provisioning role. |
| 2026-11-18 | [The Twelve-Factor App](https://12factor.net/) | devsecops | kept | Foundational methodology/principles document; distinct type from all the tool-specific resources already filed. |
| 2026-11-18 | [Terraform Best Practices](https://www.terraform-best-practices.com/) | devsecops/terraform | kept | Code-quality/best-practices guide, distinct from the official getting-started tutorial. |
| 2026-11-18 | [DORA](https://dora.dev/) | devsecops | kept | DevOps performance metrics/capabilities framework; distinct focus (measurement) from Twelve-Factor App (architecture). |
| 2026-11-18 | [CNCF Landscape](https://landscape.cncf.io/) | considered: devsecops — rejected | rejected | Unfiltered catalog of hundreds of projects, not a learning resource; notoriously overwhelming, works against the curated/lean goal. |
| 2026-11-18 | [TryHackMe](https://tryhackme.com/) | cyber | kept | Broad guided hands-on platform across many cyber domains; distinct from Bandit's narrow scope and Messer's theory focus. Reordered cyber list: TryHackMe, Professor Messer, Bandit. |
| 2026-11-18 | [KodeKloud](https://kodekloud.com/) | devsecops | kept | Free browser-based playgrounds across multiple devsecops tools; distinct type (live practice env) from curriculum/Q&A resources already filed. Note: some courses paywalled, playgrounds free. |
| 2026-11-18 | [HTB Academy](https://academy.hackthebox.com/) | cyber | kept | More rigorous/technical pentesting depth, the next step up from TryHackMe rather than a duplicate. Reordered: TryHackMe, Professor Messer, HTB Academy, Bandit. |
| 2026-11-18 | [Snyk Learn](https://learn.snyk.io/catalog/) | devsecops | kept | Fills explicit gap in devsecops scope: dependency/supply-chain and container/IaC security, distinct from Semgrep's SAST focus. |
| 2026-11-18 | [OST2 (OpenSecurityTraining2)](https://ost2.fyi/) | cyber/reverse-engineering | kept | Free university-level RE/exploit-dev/OS-internals training; created cyber/reverse-engineering subcategory, matching user's earlier example. |
| 2026-11-18 | [LFD121: Developing Secure Software](https://training.linuxfoundation.org/training/developing-secure-software-lfd121/) | devsecops | kept | Broader formal SDLC-wide course (OpenSSF cert prereq), distinct from Semgrep's hands-on vulnerability-class labs. |
| 2026-11-18 | [Hacker101](https://www.hacker101.com/) | cyber/ctfs | kept | Bug-bounty-focused web security training + own CTF; distinct angle from broader pentesting platforms. Restructured cyber: created cyber/ctfs subcategory (type-based grouping) for TryHackMe, HTB Academy, Bandit, Hacker101; Professor Messer stays top-level as the theory resource. |
| 2026-11-18 | [GitHub Skills](https://learn.github.com/skills) | devsecops/git | kept | Hands-on courses inside real GitHub repos (platform workflows), distinct from generic git knowledge already filed. |
| 2026-11-18 | [DevOps with Kubernetes (U. Helsinki)](https://courses.mooc.fi/org/uh-cs/courses/devops-with-kubernetes-2026) | devsecops/kubernetes | kept | Project-based university course (build/deploy real apps), distinct from cert-style LFS158x and internals-focused Hard Way. |
| 2026-11-18 | [DevOps with Docker (U. Helsinki)](https://courses.mooc.fi/org/uh-cs/courses/devops-with-docker-spring-2026) | devsecops/docker | kept | Deeper university-level course, distinct tier from docker-curriculum.com's lighter community tutorial. |
| 2026-11-18 | [CICD-Goat](https://github.com/cider-security-research/cicd-goat) | devsecops/ci-cd | kept | Deliberately vulnerable CI/CD environment for hands-on pipeline-security practice; fills gap, everything else there is just platform docs. |
| 2026-11-18 | [flaws.cloud](http://flaws.cloud/) | cyber/ctfs | kept | Classic AWS misconfig wargame, cloud-security equivalent of Bandit; fills gap, nothing in ctfs covers cloud yet. |
| 2026-11-18 | [Killercoda](https://killercoda.com/) | considered: devsecops — rejected | rejected | Free scenario-based sandbox practice; doesn't clearly add something unique over KodeKloud's free playgrounds covering the same tools. |
| 2026-11-18 | [Kubernetes Goat](https://github.com/madhuakula/kubernetes-goat) | devsecops/kubernetes | kept | Vulnerable-by-design K8s cluster for security practice; fills the attack/defend gap, same role CICD-Goat fills for ci-cd. |
| 2026-11-18 | [AWSGoat](https://github.com/ine-labs/AWSGoat) | cyber/ctfs | kept | Self-deployed, modern/complex AWS attack surface (serverless), distinct tier from flaws.cloud's classic fixed scenarios. |
| 2026-11-18 | [Killercoda](https://killercoda.com/) | devsecops | kept (corrected) | User overrode the earlier rejection: a well-regarded resource is worth keeping even with functional overlap. Rubric updated accordingly. |
| 2026-11-18 | [Play with Docker](https://labs.play-with-docker.com/) | devsecops/docker | kept (corrected) | Same correction as Killercoda. |
| 2026-11-18 | [Play with K8s](https://labs.play-with-k8s.com/) | devsecops/kubernetes | kept (corrected) | Same correction as Killercoda. |
| 2026-11-18 | [TerraGoat](https://github.com/bridgecrewio/terragoat) | devsecops/terraform | kept | Deliberately insecure Terraform templates; fills the attack/defend gap, same role as CICD-Goat and Kubernetes-Goat. |
| 2026-11-18 | [GitHub Code Security](https://docs.github.com/en/code-security) | devsecops/git | kept | Official docs for Dependabot/CodeQL/secret scanning; credible and widely used, kept on merits per updated rubric. |
| 2026-11-18 | [explainshell.com](https://explainshell.com/) | general | kept | Classic shell-command breakdown tool; complements linuxcommand.org. |
| 2026-11-18 | [kubectl Quick Reference](https://kubernetes.io/docs/reference/kubectl/quick-reference/) | devsecops/kubernetes | kept | Official cheat sheet, same quick-lookup role as Oh Shit Git for git. |
| 2026-11-18 | [The Book of Secret Knowledge](https://github.com/trimstray/the-book-of-secret-knowledge) | cyber | kept | Widely-praised sysadmin/security tips compilation; reference-style, distinct enough from catalog-type rejections (CNCF Landscape, Awesome-Selfhosted). |
| 2026-11-18 | [crontab.guru](https://crontab.guru/) | general | kept | Classic interactive cron-expression tool; same small-utility role as explainshell. |
| 2026-11-18 | [The Phoenix Project (excerpt)](http://images.itrevolution.com/documents/The_Phoenix_Project_excerpt.pdf) | devsecops | kept | Canonical DevOps novel excerpt; same foundational-philosophy role as Twelve-Factor App and DORA. |
| 2026-11-18 | [Continuous Delivery (official preview)](https://api.pageplace.de/preview/DT0400.9781492056676_A49444847/preview-9781492056676_A49444847.pdf) | devsecops | kept | Legitimate official publisher preview (PagePlace), replacing the earlier pirated copy of the same book. |
| 2026-11-18 | The DevOps Handbook (Kim, Humble, Debois, Willis) | devsecops | kept (corrected) | No legitimate link available (pirated mirror declined); user asked to keep books unlinked (title + author) rather than skip. Rubric updated. |
| 2026-11-18 | Threat Modeling: Designing for Security (Shostack) | devsecops | kept (corrected) | Same correction as The DevOps Handbook — listed unlinked. |
| 2026-11-18 | Hacking Kubernetes (Martin, Hausenblas) | devsecops/kubernetes | kept | Unauthorized mirror given, listed unlinked per book convention. |
| 2026-11-18 | The Web Application Hacker's Handbook, 2nd Ed. (Stuttard, Pinto) | cyber | kept | Classic web appsec/pentesting book; unauthorized mirror given, listed unlinked. |
| 2026-11-18 | [DevOps Toolkit](https://www.youtube.com/@DevOpsToolkit) | devsecops/practice | kept | Well-regarded, continuously updated DevOps YouTube channel. Restructured devsecops: split the 13-item top-level resources list into devsecops/reading (books/methodology), devsecops/secure-coding (appsec), and devsecops/practice (curricula/sandboxes/exercise banks/channels), type-based like cyber/ctfs. |
| 2026-11-18 | [freeCodeCamp](https://www.youtube.com/@freecodecamp) | general | kept | Massive, highly-regarded free course channel spanning most fields; cross-field, same home as roadmap.sh. |
| 2026-11-18 | [IppSec](https://www.youtube.com/@ippsec) | cyber/ctfs | kept | Legendary HTB walkthrough channel, tightly coupled to the HTB-style practice already filed. |
| 2026-11-18 | [John Hammond](https://www.youtube.com/@_JohnHammond) | cyber | kept | Broad infosec channel (CTFs, malware analysis, scripting), not tied to one niche, so top-level. |
| 2026-11-18 | [LiveOverflow](https://www.youtube.com/@LiveOverflow) | cyber/reverse-engineering | kept | One of the best binary exploitation/RE channels; fits the existing subcategory directly. |
| 2026-11-18 | [LearnLinuxTV](https://www.youtube.com/@LearnLinuxTV) | general | kept | Well-regarded Linux sysadmin/networking/self-hosting channel; fits the Linux cluster in general. |
| 2026-11-18 | [OWASP (official channel)](https://www.youtube.com/@OWASPGLOBAL) | devsecops/secure-coding | kept | Official OWASP content (Top 10, secure coding talks); fits the existing secure-coding subcategory. |
| 2026-11-18 | [TechWorld with Nana](https://www.youtube.com/@TechWorldwithNana) | devsecops/practice | kept | Hugely popular approachable DevOps channel; same role as DevOps Toolkit. |
| 2026-11-18 | [TechnoTim](https://www.youtube.com/@TechnoTim) | devsecops/practice | kept | Popular homelab/self-hosting channel (K8s, Docker, Proxmox, networking). |
| 2026-11-18 | [Marcel Dempers](https://www.youtube.com/@MarcelDempers) | devsecops/practice | kept | In-depth practical Docker/Kubernetes/cloud/CI-CD video series. |
| 2026-11-18 | [CNCF](https://www.youtube.com/@cncf) | devsecops/practice | kept | Official KubeCon/CloudNativeCon talks and project deep-dives. |
| 2026-11-18 | — | general/linux | restructure | Split general: created general/linux for linuxcommand.org, explainshell, crontab.guru, LearnLinuxTV; roadmap.sh and freeCodeCamp stay top-level as the orientation-across-fields cluster. |
| 2026-11-18 | [Teach Yourself CS](https://teachyourselfcs.com/) | general | kept | Curated CS fundamentals reading list; same orientation role as roadmap.sh. |
| 2026-11-18 | [The Missing Semester (MIT)](https://missing.csail.mit.edu/) | general | kept | Free MIT course on practical CS skills (shell, git, vim, debugging); broader than the Linux cluster alone, so top-level. |
| 2026-11-18 | [Boot.dev](https://www.boot.dev/) | general | kept | Gamified backend fundamentals platform (Go, Python, APIs, databases); fits the programming-fundamentals cluster. |
| 2026-11-18 | [Oh My Git!](https://ohmygit.org/) | devsecops/git | kept | Free open-source game teaching git; distinct format from everything else filed there. |
| 2026-11-18 | [DevHints](https://devhints.io/) | general | kept | Broad cross-field quick-reference cheat sheet collection. |
| 2026-11-18 | [DevDocs](https://devdocs.io/) | general | kept | Combined official-docs browser; distinct from DevHints' condensed cheat sheets. |
| 2026-11-18 | [roadmap.sh: Projects](https://roadmap.sh/projects) | general | kept | Project-ideas feature of roadmap.sh, distinct purpose (practice/build) from the roadmaps already filed. |
| 2026-11-18 | [Project Based Learning](https://github.com/practical-tutorials/project-based-learning) | general | kept | Guided build-along tutorials across languages; distinct from roadmap.sh/projects' self-directed idea list. |
| 2026-11-18 | [Build Your Own X](https://github.com/codecrafters-io/build-your-own-x) | general | kept | Reimplement-real-tools genre, distinct pedagogical angle (clone to learn internals) from general project tutorials. |
| 2026-11-18 | [The Odin Project](https://www.theodinproject.com/) | general | kept | Free, structured, project-based full-stack web dev curriculum; distinct structure from freeCodeCamp's course-library format. |
| 2026-11-18 | — | software-dev | restructure | Created new top-level category software-dev (web/mobile/desktop/general software development), at user's request. Moved freeCodeCamp, Boot.dev, roadmap.sh/projects, Project Based Learning, Build Your Own X, The Odin Project out of general into software-dev; created software-dev/web for Odin Project. general keeps roadmap.sh, Teach Yourself CS, Missing Semester, DevHints, DevDocs, and the linux subcategory. |
| 2026-11-18 | [Eloquent JavaScript](https://eloquentjavascript.net/) | software-dev/web | kept | Free, well-regarded JS fundamentals + browser/DOM book. |
| 2026-11-18 | [Frontend Mentor](https://www.frontendmentor.io/) | software-dev/web | kept | Real-world front-end build challenges from provided designs. |
| 2026-11-18 | [Flexbox Froggy](https://flexboxfroggy.com/) | software-dev/web | kept | Classic CSS Flexbox game. |
| 2026-11-18 | [CSS Battle](https://cssbattle.dev/) | software-dev/web | kept | Competitive CSS code-golf challenges; distinct open-ended format from Flexbox Froggy. |
| 2026-11-18 | [Free Programming Books](https://github.com/EbookFoundation/free-programming-books) | software-dev | kept | Massive curated free-book list by language; broader than web, top-level. |
| 2026-11-18 | [Beej's Guides](https://beej.us/guide/) | software-dev | kept | Classic systems-programming guides (network programming, C, Unix IPC). |
| 2026-11-18 | — | general | correction | User corrected scope: software-dev is strictly application-level (web/mobile/desktop), not systems/infra/networking. Moved Build Your Own X, Free Programming Books, Beej's Guides, and Project Based Learning from software-dev into general. software-dev narrowed to freeCodeCamp, Boot.dev, roadmap.sh/projects, plus the web subcategory. |
| 2026-11-18 | [How to Design Programs](https://htdp.org/) | general | kept | Classic program-design/functional-programming fundamentals book; CS methodology, not application-level. |
| 2026-11-18 | [SICP](https://sarabander.github.io/sicp/) | general | kept | Legendary MIT CS textbook; deeper tier than HtDP, same foundational-CS cluster. |
| 2026-11-18 | [free-for-dev](https://github.com/ripienaar/free-for-dev) | general | kept | Practical list of free dev/cloud tool tiers; cross-cutting utility, not catalog-overwhelm (distinct from CNCF Landscape/Awesome-Selfhosted rejections). |
| 2026-11-18 | [Computerphile](https://www.youtube.com/@Computerphile) | computer-science | kept | Well-known accessible CS concepts channel. Created new top-level category computer-science (CS theory/fundamentals), at user's request, moving Teach Yourself CS, How to Design Programs, and SICP out of general; general's description narrowed to tools/references/career (general itself was NOT removed, only re-scoped — user flagged confusion here). |
| 2026-11-18 | [Fireship](https://www.youtube.com/@Fireship) | software-dev | kept | Fast-paced web/app dev + tooling channel. |
| 2026-11-18 | [Ben Eater](https://www.youtube.com/@BenEater) | computer-science | kept (corrected) | — |
| 2026-11-18 | [Hussein Nasser (hnasr)](https://www.youtube.com/@hnasr) | systems | kept | Deep technical databases/networking/systems-design channel. Created new top-level category systems (applied hardware/OS/networking, distinct from computer-science theory), at user's correction. Moved Ben Eater, Beej's Guides, Build Your Own X into systems. |
| 2026-11-18 | [The Coding Train](https://www.youtube.com/@TheCodingTrain) | computer-science | kept | Algorithms/programming fundamentals taught through creative coding; algorithmic-thinking focus over app-building. |
| 2026-11-18 | [Tech With Tim](https://www.youtube.com/@TechWithTim) | software-dev | kept | Python/general programming taught via real project building. |
| 2026-11-18 | [CS50 (Harvard)](https://www.youtube.com/cs50) | computer-science | kept | The legendary intro CS course. |
| 2026-11-18 | [Python Tutor](https://pythontutor.com/) | computer-science | kept | Classic code-execution visualizer, pairs with intro CS courses like CS50. |
| 2026-11-18 | [Automate the Boring Stuff with Python](https://automatetheboringstuff.com/) | general | kept | Practical Python scripting/automation book, not application-building or CS theory. |
| 2026-11-18 | [Real Python](https://realpython.com/) | general | kept | Comprehensive Python tutorial hub, same language-learning role as Automate the Boring Stuff. |
| 2026-11-18 | [Rustfinity](https://www.rustfinity.com/) | general/languages/rust | kept | Broader interactive Rust challenge platform. |
| 2026-11-18 | [Rustlings](https://github.com/rust-lang/rustlings) | general/languages/rust | kept | Official small Rust syntax exercises. |
| 2026-11-18 | [The Rust Book](https://doc.rust-lang.org/book/) | general/languages/rust | kept | Official comprehensive Rust guide. Created general/languages subcategory (python, rust, go) given the growing per-language cluster, same pattern as general/linux. Moved Automate the Boring Stuff + Real Python into general/languages/python. |
| 2026-11-18 | [Go by Example](https://gobyexample.com/) | general/languages/go | kept | Classic example-driven Go reference. |
| 2026-11-18 | [Learn X in Y Minutes](https://learnxinyminutes.com/) | general/languages | kept | Cross-language syntax overviews; not language-specific, so top of languages subcategory. |
| 2026-11-18 | [A Tour of Go](https://go.dev/tour/welcome/1) | general/languages/go | kept | Official interactive Go tutorial. |
| 2026-11-18 | [Advent of Code](https://adventofcode.com/) | competitive-programming | kept | Created new top-level category competitive-programming, at user's request. |
| 2026-11-18 | [CSES Problem Set](https://cses.fi/problemset/) | competitive-programming | kept | Classic algorithm-topic-organized practice problems, distinct structured format from AoC's themed daily puzzles. |
| 2026-11-18 | [AtCoder](https://atcoder.jp/) | competitive-programming | kept | Major rated-contest platform; distinct live/ranked format from CSES (untimed practice) and AoC (themed puzzles). |
| 2026-11-18 | [Codewars](https://www.codewars.com/) | competitive-programming | kept | Bite-sized kata with ranking system, casual daily-practice format distinct from timed contests. |
| 2026-11-18 | [HackerRank](https://www.hackerrank.com/) | competitive-programming | kept | Broad platform (algorithms, SQL, interview prep, recruiting assessments); distinct interview-prep angle. |
| 2026-11-18 | [NeetCode](https://neetcode.io/) | competitive-programming | kept | Curated interview-prep roadmap with video explanations, more structured than HackerRank. |
| 2026-11-18 | [LeetCode](https://leetcode.com/) | competitive-programming | kept | The essential interview-prep problem platform itself, which NeetCode's roadmap is built on top of; reordered to near the top given how fundamental it is. |
| 2026-11-18 | [regex101](https://regex101.com/) | general/regex | kept | Interactive regex tester/debugger. |
| 2026-11-18 | [Regex Crossword](https://regexcrossword.com/) | general/regex | kept | Puzzle-game regex practice. |
| 2026-11-18 | [RegexOne](https://regexone.com/) | general/regex | kept | Structured regex lessons. Created general/regex subcategory for the three-item cluster. |
| 2026-11-18 | [OpenVim](https://openvim.com/) | general/linux | kept | Interactive Vim tutorial, terminal-skills scope. |
| 2026-11-18 | [Vim Adventures](https://vim-adventures.com/) | general/linux | kept | Game-based Vim learning, distinct format from OpenVim. |
| 2026-11-18 | [Algorithms (Jeff Erickson)](https://jeffe.cs.illinois.edu/teaching/algorithms/) | computer-science | kept | Free university-level algorithms textbook. |
| 2026-11-18 | [Big-O Cheat Sheet](https://www.bigocheatsheet.com/) | computer-science | kept | Classic complexity quick-reference, companion to the algorithms textbook. |
| 2026-11-18 | [Open Data Structures](https://opendatastructures.org/) | computer-science | kept | Free data structures textbook, complements the algorithms textbook. |
| 2026-11-18 | [Algorithm Visualizer](https://algorithm-visualizer.org/) | computer-science | kept | Interactive algorithm-execution animator. |
| 2026-11-18 | [VisuAlgo](https://visualgo.net/en) | computer-science | kept | Widely-used algorithm/DS visualizer, popular for CP; kept alongside Algorithm Visualizer per "good on its own merits" rule. |
| 2026-11-18 | [The Fuzzing Book](https://www.fuzzingbook.org/) | devsecops/secure-coding | kept | Academic fuzzing/test-generation book, framed as SDLC testing methodology. |
| 2026-11-18 | [Cryptopals](https://cryptopals.com/) | cyber/ctfs | kept | Hands-on cryptography-breaking challenge set; same practice-platform format as Bandit, crypto-focused. |
| 2026-11-18 | [pwn.college](https://pwn.college/) | cyber/reverse-engineering | kept | University-affiliated hands-on binary exploitation/systems security training. |
| 2026-11-18 | [MalwareUnicorn](https://malwareunicorn.org/#/) | cyber/reverse-engineering | kept | Well-known hands-on malware analysis workshops. |
| 2026-11-18 | [Microcorruption](https://microcorruption.com/) | cyber/reverse-engineering | kept | Classic embedded/firmware RE wargame. |
| 2026-11-18 | [picoCTF](https://picoctf.org/) | cyber/ctfs | kept | CMU's popular beginner-friendly CTF archive + annual competition. |
| 2026-11-18 | [Root-Me](https://www.root-me.org/?lang=en) | cyber/ctfs | kept | Large long-standing multi-category challenge platform. |
| 2026-11-18 | [Google CTF](https://capturetheflag.withgoogle.com/) | cyber/ctfs | kept | Google's official CTF competition/archive. |
| 2026-11-18 | [CTFtime](https://ctftime.org/) | cyber/ctfs | kept | Central CTF calendar/rankings/writeup hub; distinct aggregator type. |
| 2026-11-18 | [Practical Networking](https://www.practicalnetworking.net/) | systems | kept | Applied networking fundamentals (TCP/IP, subnetting, routing). |
| 2026-11-18 | [The Cherno](https://www.youtube.com/@TheCherno) | general/languages/cpp | kept | User-flagged principle: categorize by what a resource is PRIMARILY about, not every field it's useful for. The Cherno is primarily general C++ education (the game-engine series is one side series), so it's a language resource, not game-dev. Created general/languages/cpp. |
| 2026-11-18 | [javidx9](https://www.youtube.com/@javidx9) | game-dev/foundations | kept | Unlike The Cherno, javidx9's primary content IS building games/renderers from scratch — genuinely game-dev-specific, correctly stays in game-dev. |
| 2026-11-18 | [A Theory of Fun for Game Design](https://www.theoryoffun.com/) | game-dev/design | kept | Legendary game design theory book. |
| 2026-11-18 | [The Art of Game Design](https://www.artofgamedesign.com/) | game-dev/design | kept | Legendary "100 lenses" game design book. |
| 2026-11-18 | [Hands-on Rust](https://pragprog.com/titles/hwrust/hands-on-rust/) | game-dev/engines | kept | Structured entirely around building a roguelike; game-dev-specific despite teaching Rust along the way. |
| 2026-11-18 | [Game Engine Architecture](https://www.gameenginebook.com/) | game-dev/foundations | kept | Legendary industry-standard engine architecture textbook. |
| 2026-11-18 | [Handmade Hero](https://handmadehero.org/) | game-dev/foundations | kept | Legendary from-scratch engine/game build series. |
| 2026-11-18 | [Game Engine Black Book](https://fabiensanglard.net/gebb/) | game-dev/foundations | kept | Deep technical breakdowns of classic engines (Wolfenstein 3D, DOOM). |
| 2026-11-18 | [Data-Oriented Design](https://www.dataorienteddesign.com/dodbook/) | game-dev/foundations | kept | Performance-focused design paradigm central to engine architecture. |
| 2026-11-18 | [MIT 6.837: Computer Graphics](https://ocw.mit.edu/courses/6-837-computer-graphics-fall-2012/) | game-dev/foundations | kept | Official MIT OCW graphics course. |
| 2026-11-18 | [GAMES101](https://sites.cs.ucsb.edu/~lingqi/teaching/games101.html) | game-dev/foundations | kept | Extremely popular free comprehensive graphics course. |
| 2026-11-18 | [vkguide](https://vkguide.dev/) | game-dev/engines | kept | Modern practical Vulkan renderer tutorial, complements Vulkan Tutorial. |
| 2026-11-18 | — | — | restructure | "Make it impeccable" full-repo pass: verified every internal link resolves (none broken), checked for duplicate URLs across the whole repo (none found), verified every breadcrumb points to the correct parent. Found and fixed two subcategories that had blown past the 15-item threshold: split game-dev/engines (24 items) into godot/, unity/, graphics-programming/ + a trimmed top-level list; split game-dev/foundations (23 items) into graphics/, engine-architecture/, math-and-simulation/, ai-and-procedural/. Added a .gitignore excluding AI-assistant/session artifacts (.claude/, etc. — distinct from the ai/ category folder, no collision). Added the "file by what it's primarily about" principle to CONTRIBUTING.md explicitly (from the Cherno correction). No other miscategorizations found. |
| 2026-11-18 | — | game-dev, ai | restructure | Built out game-dev from scratch (previously empty) across a long resource-review session: MakeCode Arcade, Bitsy, Twine → no-code; Godot, Unity Learn, Pygame, Phaser, LÖVE2D, Defold, raylib, MonoGame, Bevy + cheat book, Three.js Journey, Box2D, Catlike Coding, WebGL2 Fundamentals, LearnOpenGL, Vulkan Tutorial, LearnWebGPU, RogueLike Tutorials, Godot Demo Projects, Brackeys, Code Monkey, Heartbeast → engines; Game Programming Patterns, Red Blob Games, Nature of Code, 3Blue1Brown Linear Algebra, Immersive Math, Allen Chou Physics, Game AI Pro, PCG Book, Ray Tracing in One Weekend, Computer Graphics from Scratch, Scratchapixel, Inigo Quilez, Lode's CG Tutorial, TinyRenderer, Sebastian Lague, Freya Holmér → foundations; Draw a Box, Ctrl+Paint, Blender Studio Training, Lospec, Slynyrd, Saint11, CG Cookie → art; The Game Audio Tutorial, Audiokinetic Wwise → audio; Game Design Concepts, Game Balance Concepts, Level Design Book, GMTK → design; Ludum Dare, itch.io Jams, Global Game Jam, Godot Wild Jams, JS13K, 7DRL → jams; Gaffer On Games, Fast-Paced Multiplayer, Valve Source Networking, Godot Multiplayer, Colyseus, Mirror, GGPO → networking; How To Market A Game, Steamworks, itch.io Creator Docs → publishing; GameDev.tv, CS50 Games, GDC Vault stayed top-level (broad, cross-subcategory). Also created a new empty top-level `ai` category per user's request, to be filled when AI resources come in. Also did a full-repo revision pass earlier in the session (see prior restructure entry). |
| 2026-11-18 | — | — | restructure | Full repo revision pass: fixed stale cross-reference in software-dev/README.md (systems/networking used to point to `general`, now correctly points to `systems`), trimmed an overclaiming line in competitive-programming's LeetCode entry, renamed gamedev/ to game-dev/ for naming consistency with other multi-word categories (updated Home README link). No other miscategorizations or duplicates found on review. |
| 2026-11-18 | [MakeCode Arcade](https://arcade.makecode.com/) | game-dev | kept | Approachable block/code retro game maker; first game-dev resources. |
| 2026-11-18 | [Bitsy](https://www.bitsy.org/) | game-dev | kept | Extremely simple tiny story-game maker. |
| 2026-11-18 | [Twine](https://twinery.org/) | game-dev | kept | Interactive fiction/branching narrative tool, no coding required. |
| 2026-11-18 | [Godot: Getting Started](https://docs.godotengine.org/en/stable/getting_started/introduction/index.html) | game-dev | kept | Free open-source game engine docs; first real engine, distinct tier from the no-code tools. |
| 2026-11-18 | [Unity Learn](https://learn.unity.com/) | game-dev | kept | Official learning platform for Unity, the industry-standard commercial engine; distinct ecosystem from Godot. |
| 2026-11-18 | [GameDev.tv](https://www.gamedev.tv/) | game-dev | kept | Broad cross-engine game dev education platform. |
| 2026-11-18 | [Making Games with Python & Pygame](https://inventwithpython.com/pygame/) | game-dev | kept | Free beginner-friendly Pygame book; distinct Python-based ecosystem. |
| 2026-11-18 | [Phaser Tutorials](https://phaser.io/tutorials) | game-dev | kept | Official tutorials for the web/JS game framework; distinct ecosystem. Cluster forming: no-code tools, full engines, code libraries — flagged for a possible future split, not acted on yet. |

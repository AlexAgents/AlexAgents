<img src="banner.jpg" width="100%" alt="banner" />

<h1 align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=JetBrains+Mono&weight=700&size=28&pause=1000&color=4FC3F7&center=true&vCenter=true&width=680&lines=Hi%2C+I'm+Alexey+Q+%F0%9F%91%8B;System+%26+Business+Analyst;Python+for+data+%26+automation;I+speak+both+business+and+code" alt="Typing SVG" />
</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/SQL-30363d?style=flat-square&logo=postgresql&logoColor=4FC3F7" />
  <img src="https://img.shields.io/badge/BPMN%202.0-30363d?style=flat-square" />
  <img src="https://img.shields.io/badge/UML%20%2F%20ERD-30363d?style=flat-square" />
  <img src="https://img.shields.io/badge/PlantUML-30363d?style=flat-square" />
  <img src="https://img.shields.io/badge/REST%20API-30363d?style=flat-square" />
  <img src="https://img.shields.io/badge/Postman-30363d?style=flat-square&logo=postman&logoColor=FF6C37" />
  <img src="https://img.shields.io/badge/Jira-30363d?style=flat-square&logo=jira&logoColor=2684FF" />
  <img src="https://img.shields.io/badge/Confluence-30363d?style=flat-square&logo=confluence&logoColor=2684FF" />
  <img src="https://img.shields.io/badge/pandas-30363d?style=flat-square&logo=pandas&logoColor=E70488" />
  <img src="https://img.shields.io/badge/Git-30363d?style=flat-square&logo=git&logoColor=F05032" />
</p>

## 🧠 Analyst who codes

```python
class Analyst:
    def __init__(self):
        self.name = "Alexey Q"
        self.role = "System / Business Analyst"
        self.motto = "A good spec is a bug that never happened."

        self.deliverables = [
            "requirements (BRD / SRS)", "user stories & acceptance criteria",
            "process models (BPMN)", "data & system models (UML / C4)",
            "architecture decisions (ADR)", "threat models (STRIDE)",
            "API / integration specs", "UI specs & prototypes",
        ]
        self.toolkit = ["Python", "SQL", "pandas", "REST", "Git", "C++ (low-level / when needed)"]
        self.domains = ["fintech / data", "automation", "AI/ML integration"]

    def value(self):
        return "I translate vague 'make it work' into clear, testable specs — " \
               "and can prototype the tricky parts myself."
```

## 🧭 How I work

- **Remove uncertainty.** Turn stakeholder "wishlists" into formal requirements and acceptance criteria.
- **Draw, don't tell.** Processes in BPMN, data & systems in UML/C4, integrations in API specs, decisions in ADRs.
- **Prototype the fuzzy parts.** When a requirement is vague, I throw together a Python PoC to validate it on real data before dev spends a sprint.
- **Speak two languages.** With business — value and risk; with engineering — contracts, data models, edge cases.

## 🔎 Flagship case study · MYCELIUM CORE

<p align="center">
  <img src="https://raw.githubusercontent.com/AlexAgents/mycelium-core/main/mycelium-core/src/assets/icons/Original.png" width="64" alt="MYCELIUM CORE logo" />
</p>

<p align="center">
  <a href="https://github.com/AlexAgents/mycelium-core"><img src="https://img.shields.io/badge/Python%203.11+-3776AB?style=flat-square&logo=python&logoColor=white" /></a>
  <a href="https://docs.soliditylang.org/en/v0.8.20/"><img src="https://img.shields.io/badge/Solidity%200.8.20-363636?style=flat-square&logo=solidity&logoColor=white" /></a>
  <a href="https://github.com/AlexAgents/mycelium-core/tree/main/mycelium-core/tests"><img src="https://img.shields.io/badge/Tests-180%20passed-success?style=flat-square" /></a>
  <a href="https://www.figma.com/design/PWzJmLP7TrrbjcL6F85KoU/mycelium-core"><img src="https://img.shields.io/badge/Figma-Mockups-F24E1E?style=flat-square&logo=figma&logoColor=white" /></a>
  <a href="https://github.com/AlexAgents/mycelium-core/tree/main/docs"><img src="https://img.shields.io/badge/MkDocs-70%2B%20pages-0969da?style=flat-square&logo=materialformkdocs&logoColor=white" /></a>
</p>

> **Context.** A Master's degree project: model, run and *audit* an on-chain e-voting process on a local Ethereum network — and prove its correctness. The analytical challenge was to turn a security-critical, multi-stage voting protocol into unambiguous, testable requirements and architecture **before** a single line of UI code.

**What I did (as a system analyst):**

- **Requirements** — authored the SRS (project + documentation tracks).
- **Process modelling** — 6 BPMN flows: Setup, Voting, Mass Vote, Audit, Error Handling, Session Lifecycle.
- **System modelling** — 17 UML / C4 diagrams: Component, Class, Sequence, State, Activity, Use Case, Deployment, C4.
- **Architecture decisions** — 7 ADRs (e.g. strict layered architecture; Geth `--dev` mode).
- **Threat modelling** — STRIDE analysis + 6 security invariants (SEC-01..06), each enforced in-contract *and* re-checked reactively by the audit service.
- **Interface specs** — 10 core-module API references.
- **UI specification** — Figma mockups (4 tabs, 5 dialog types), a design system, 53 annotated notes.
- **Verification** — translated invariants into **180** unit + integration tests against a real Geth node: requirements *proved*, not just written.
- **Documentation** — 70+ page MkDocs site (EN/RU), glossary (33 terms), FAQ (16).

> **Outcome.** A layered design where the UI layer is **forbidden** to import Web3 / Solidity / crypto directly; every security rule is double-guarded (proactive in contract + reactive in audit); the spec is complete enough to serve as a Master's deliverable **and** a reference SA artifact set.

<details>
<summary>📦 Artifact catalog (delivered)</summary>

| Area | Delivered | Link |
|------|-----------|------|
| Requirements | SRS (project + docs) · glossary (33) · FAQ (16) | [SRS](https://github.com/AlexAgents/mycelium-core/blob/main/docs/src/reference/srs.ru.md) |
| Process models | 6 BPMN flows | [Catalog](https://github.com/AlexAgents/mycelium-core/blob/main/docs/src/diagrams/index.ru.md) |
| System models | 17 UML / C4 diagrams | [Catalog](https://github.com/AlexAgents/mycelium-core/blob/main/docs/src/diagrams/index.ru.md) |
| Architecture | Layered arch + 7 ADRs | [Overview](https://github.com/AlexAgents/mycelium-core/blob/main/docs/src/architecture/overview.ru.md) |
| Security | STRIDE + 6 invariants (SEC-01..06) | [Threat model](https://github.com/AlexAgents/mycelium-core/blob/main/docs/src/security/threat-model.ru.md) |
| Interface | 10 API specs · Figma (53 notes) · design system | [Figma](https://www.figma.com/design/PWzJmLP7TrrbjcL6F85KoU/mycelium-core) |
| Verification | 180 tests (unit + integration, real Geth) | [Tests](https://github.com/AlexAgents/mycelium-core/tree/main/mycelium-core/tests) |
| Docs site | 70+ pages, EN/RU (MkDocs) | [Docs](https://github.com/AlexAgents/mycelium-core/blob/main/docs/src/index.ru.md) |

</details>

<details>
<summary>🖼️ UI proof — Admin tab (dark / light)</summary>

<table>
<tr>
<th align="center">Dark</th>
<th align="center">Light</th>
</tr>
<tr>
<td align="center"><img src="https://raw.githubusercontent.com/AlexAgents/mycelium-core/main/docs/src/assets/images/screenshots/admin-tab-dark.png" alt="Admin dark" width="420"></td>
<td align="center"><img src="https://raw.githubusercontent.com/AlexAgents/mycelium-core/main/docs/src/assets/images/screenshots/admin-tab-light.png" alt="Admin light" width="420"></td>
</tr>
</table>

</details>

<p align="center"><sub>🔗 Full project &amp; switchable EN/RU docs: <a href="https://github.com/AlexAgents/mycelium-core">github.com/AlexAgents/mycelium-core</a></sub></p>

---

## 🗺️ Roadmap 2025–2030 · Project Codenames

> *Each project has a codename. Some will ship. Some will burn beautifully.*
>
> **Status** is self-assessed (`planned` / `poc` / `wip`). The delivered reference is **MYCELIUM CORE** above; everything below is roadmap.

### 📊 Data, Automation & Analysis
| Codename | What it solves | Status |
|----------|----------------|:------:|
| `CRYPT-SIGHT` | On-chain / market data analysis & metric dashboards | poc |
| `SI-GRAB` | Collection & normalization of data from distributed sources | planned |
| `FREQ-FILTER` | Intelligent signal filtering (audio / numeric streams) | planned |
| `RISK-PYRAMID` | Risk modelling of fraudulent financial schemes (educational) | planned |

### 🤖 AI / ML & NLP — integration & requirements
| Codename | What it solves | Status |
|----------|----------------|:------:|
| `ELYSIUM-SCAN` | Spec of an AI pipeline for medical-image analysis | planned |
| `NEURO-MERGE` | Integration of AI agents into user scenarios | planned |
| `PROMPT-FORGE` | Formalization & control of generative-model parameters | wip |
| `CosmaLingua` | NLP solution for a linguistics task (UN track) | planned |

### 🧩 Process & Requirements Engineering
| Codename | What it solves | Status |
|----------|----------------|:------:|
| `CONTRACT-SCAN` | Static analysis of smart contracts for logical contradictions | planned |
| `CONTRACT-GEN` | Generation of smart contracts from business rules | planned |
| `IDEA-FORGE` | Formalizing creative methods (TRIZ, brainstorming) into algorithms | planned |
| `ANALYST-CALC` | Toolkit for a system analyst (metrics, templates) | wip |

### 🔧 Tools & Integration
| Codename | What it solves | Status |
|----------|----------------|:------:|
| `GEN-v3` | Web tool for adaptive prompt generation | wip |
| `CODE-MERGE` | Composing Python modules via natural language | planned |
| `BRACKMAN` | Personal site / integration showcase | wip |

<details>
<summary>🔬 Deep-tech R&D (C++ / algorithms)</summary>

| Codename | What it solves | Status |
|----------|----------------|:------:|
| `QUATERNARY` | Base-4 encoding & compression experiments | planned |
| `CELL-RETRO` | Low-level cellular-automata modelling | planned |
| `EPICURE` | Research 3D engine | planned |
| `BAD-UXUI` | Non-standard UI experiments | planned |
</details>

<details>
<summary>📋 Backlog & early-stage concepts</summary>

| Codename | What it solves |
|----------|----------------|
| `Genesis` / `MAYHEM` | R&D prototypes of multi-agent systems |
| `PATTERN-SYNTH` | Pattern discovery & synthesis in datasets |
| `DIFF-QR` | Automated artifact generation via generative models |
| `ETL-PROTO` | ETL pipeline prototype for ledger addresses & transactions |
| `MUSIC-META` | Analysis & generation of musical patterns |
| `SPEECH-FILTER` | Intelligent moderation of speech content |
| `MORSE-DECODER` | Automatic interpreter of Morse-code signals |
| `SPACE-PLANNER` | Parametric floor-plan generation with style visualization |
| `ACHIEVE-ENGINE` | Achievement engine for business-process gamification |
| `INTERACT-LOG` | Personal communications analytics (consent-based, local-only) |
| `POPULATION-MODEL` | Demographic modelling & scenario analysis |
| `TRUST-CURRENCY` | Concept of a trust-credit-based currency |
| `SOCIAL-HEATMAP` | Social-interaction analysis via a graph model |
| `OFFLINE-P2P` | Spec of a simple decentralized communication network |
| `US-VR-ORIENTEER` | Universal orientation model for unknown terrain |
| `GAME-ECONOMY` | In-game economy modelling with full monetization |
| `MARKET-TOP1000` | Year-over-year dynamics of top-1000 crypto assets |
</details>

## 🎯 Currently

- **Open to:** System / Business Analyst roles · fintech · data · AI/ML integration · remote
- **Reference project:** [MYCELIUM CORE](https://github.com/AlexAgents/mycelium-core) — delivered (case study ↑)
- **Sharpening:** BPMN 2.0 · IIBA BABOK · SQL window functions
- **Next on roadmap:** `MAYHEM` — R&D prototypes of multi-agent systems

<!--## 📈 Activity
Uncomment once you want the cards back; mycelium-core now gives real activity.

<p align="center">
  <img src="https://github-stats-extended.vercel.app/api?username=AlexAgents&show_icons=true&hide_border=true&bg_color=0d1117&title_color=4FC3F7&text_color=e2e8f0&icon_color=2dd4bf&border_color=0d1117" width="48%" />
  <img src="https://streak-stats.demolab.com/?user=AlexAgents&hide_border=true&background=0d1117&border=0d1117&stroke=4FC3F7&ring=4FC3F7&fire=2dd4bf&currStreakNum=4FC3F7&currStreakLabel=4FC3F7&sideNums=e2e8f0&sideLabels=e2e8f0&dates=94a3b8" width="48%" />
</p>
<p align="center">
  <img src="https://github-stats-extended.vercel.app/api/top-langs/?username=AlexAgents&layout=compact&hide_border=true&bg_color=0d1117&title_color=4FC3F7&text_color=e2e8f0&border_color=0d1117" width="40%" />
</p>
-->

---

<p align="center">
  <i>Requirements first. Code when it earns its place.</i>
</p>
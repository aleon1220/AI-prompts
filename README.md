# AI-prompts
library AI Prompts and use cases
This repository is intended to store markdown prompt files for different projects.

---

## 🧭 Architecture & Quick Navigation

This library is organized into **5 Functional Domains** and classified across **3 Complexity Tiers** (`🟢 Quick`, `🔵 Structured`, `🟣 System`) so you can locate the right prompt in seconds.

- 📖 **[Master Prompt & Use-Case Catalog (`CATALOG.md`)](./CATALOG.md)** — Single-page searchable table & *"I want to..."* decision matrix across every file in the repository.
- 📐 **[Engineering Standards & Taxonomy (`STANDARDS.md`)](./STANDARDS.md)** — Folder taxonomy, 3-tier prompt maturity standard, metadata header spec, and guardrails.
- 🧩 **[Starter Templates (`templates/`)](./templates/)** — Ready-to-copy [`prompt-template.md`](./templates/prompt-template.md) and [`use-case-template.md`](./templates/use-case-template.md).

### Repository Map by Domain

| Domain | Category Folders | Primary Use Cases |
| :--- | :--- | :--- |
| **1. Engineering, SDLC & Operations** | [`software-development-lifecycle/`](./software-development-lifecycle/)<br>[`troubleshooting-debugging/`](./troubleshooting-debugging/) | Git commit generation (standard, <40w, Jira `D09-`), Bitbucket PR summaries, CI/CD pipeline log debugging, and multi-file service migration audits. |
| **2. Meetings, Collaboration & Comms** | [`meetings/`](./meetings/)<br>[`chat-analysis/`](./chat-analysis/) | Auditable MS Teams meeting minutes (with `[hh:mm:ss]` citations & confidence scoring), prioritized action tables, tone/dynamics analysis, and project chat Q&A. |
| **3. Productivity, Tasks & Retrospectives** | [`retrospectives/`](./retrospectives/)<br>[`task-management/`](./task-management/)<br>[`office365-copilot/`](./office365-copilot/) | Daily/weekly/monthly Markdown worklog reflection (Deep Work, GTD, PARA, WBS alignment, Mermaid visualizations) and M365 Copilot email-to-task checklists. |
| **4. Content, Document & Learning Intelligence** | [`content-summarization/`](./content-summarization/)<br>[`pdfs/`](./pdfs/)<br>[`policies/`](./policies/)<br>[`training-and-learning/`](./training-and-learning/) | Summarizing technical training videos, Confluence PDF exports, privacy policies, online articles, and video scripts. |
| **5. AI Strategy, Session Ops & Use Cases** | [`ai-use-cases/`](./ai-use-cases/) | Universal AI chat session audit & context hand-off prompt + 8 high-level multimodal GenAI use-case blueprints. |

---

## ⚡ Top High-Impact Prompts

1. **[MS Teams Transcript → Crisp Auditable Records](./meetings/teams-transcript-crisp-records.md)** (`🟣 System`) — Production system prompts with timestamp evidence citations, speaker alias normalization, and confidence ratings.
2. **[Monthly Worklog Reflection System Prompt](./retrospectives/worklog-monthly-reflection.md)** (`🟣 System`) — 10-section productivity coach analyzing goals, WBS timesheets, open loops, and Deep Work/GTD/PARA patterns.
3. **[Universal AI Session Audit & Hand-Off](./ai-use-cases/extract-ai-chat-achievements-todos.md)** (`🟣 System`) — Audits a long AI coding/brainstorming session into achievements, `[Explicit]`/`[Implicit]` backlogs, and a ready-to-paste context hand-off block.
4. **[Git Commit & Jira `D09-` Suite](./software-development-lifecycle/create-git-commit-messages.md)** (`🔵 Structured`) — Enforces 50/72 subject/body rules, "what & why" focus, file exclusions, and Jira key extraction.
5. **[Technical Training Session Summarizer](./training-and-learning/assess-class-training-transcript.md)** (`🔵 Structured`) — Converts engineering class transcripts into an 8-part technical study and action guide.

---

## Template to use

> [!NOTE]
> For full prompt and use-case templates with metadata headers, see [`templates/prompt-template.md`](./templates/prompt-template.md) and [`templates/use-case-template.md`](./templates/use-case-template.md). Below is the core collapsible snippet used inside prompt files:

```html
<!-- expand sections HTML in markdown -->
 
<details>
<summary> TODO Prompt Title 📝 </summary>

```text
TODO content
```
</details>

<!-- End of reusable snippet -->

```

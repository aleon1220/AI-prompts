# Meetings & MS Teams Transcript Intelligence

> **Domain:** 2. Meetings, Collaboration & Communications | **Parent Catalog:** [`../CATALOG.md`](../CATALOG.md)

A curated suite of prompts for transforming raw meeting transcripts (especially Microsoft Teams `.vtt`/`.docx` audio transcripts and meeting chat logs) into structured minutes, prioritized action tables, auditable decision logs, and follow-up communications.

---

## ⚡ Quick-Pick Decision Matrix (Which Meeting Prompt Should I Use?)

To simplify choosing among the 8 files (11 prompt variants) in this folder, pick by **Tier** and **Required Features**:

| File | Tier | Timestamp Citations `[hh:mm:ss]` | Confidence Scoring | Action Priority Table | Chat Highlights | Special Differentiator |
| :--- | :--- | :---: | :---: | :---: | :---: | :--- |
| **[`teams-transcript-crisp-records.md`](./teams-transcript-crisp-records.md)** | `🟣 System` | ✅ | ✅ | ✅ (`A-1` SMART) | ✅ (`<chat>`) | **Gold Standard:** Alias normalization (`Liz` → `Elizabeth`), revision tracking, `<metadata>`/`<transcript>`/`<chat>` blocks, worked examples (Copilot & Claude Opus 4.8 High variants) |
| **[`detailed-meeting-transcript-analysis.md`](./detailed-meeting-transcript-analysis.md)** | `🟣 System` | ✅ | ✅ | ✅ (`A-1` SMART) | ✅ | **Azure AI Foundry GPT-4o System Prompt:** Strict ISO 8601 metadata, SMART actions, sparse-data clarification fallback |
| **[`analyse-msteams-transcript.md`](./analyse-msteams-transcript.md)** | `🔵 Structured` | — | `(Inferred)` tag | ✅ (Markdown Table) | ✅ | **Action-First Layout:** Places the prioritized action table immediately after Executive Summary + AI strategic risk wrap-up (Gemini 1.5 Pro & Agenda Planner variants) |
| **[`meeting-transcript-analysis-prompt.md`](./meeting-transcript-analysis-prompt.md)** | `🔵 Structured` | — | — | ✅ | — | **Tone & Follow-Up Comms:** Evaluates participant tone shifts (with quotes) + **drafts a follow-up email / Teams post** |
| **[`summarise-msteams-meeting.md`](./summarise-msteams-meeting.md)** | `🔵 Structured` / `🟢 Quick` | — | — | ✅ | ✅ | **Dual-Purpose:** Includes both an MS Teams call minutes prompt AND a 7-question project chat transcript analyzer |
| **[`detailed-meeting-minutes.md`](./detailed-meeting-minutes.md)** | `🔵 Structured` | — | — | ✅ | ✅ | Includes **Attended vs. Invited headcount** comparison + Chat Highlights |
| **[`comprehensive-summary.md`](./comprehensive-summary.md)** | `🔵 Structured` | — | — | ✅ | — | Clean baseline minutes extracting **Speakers & Roles** (only when explicitly mentioned) |
| **[`summarise-meeting-transcript.md`](./summarise-meeting-transcript.md)** | `🟢 Quick` | — | — | Bullets | Links/Files | **Fastest 4-Part Recap:** Intro paragraph, topic/decision bullets, conclusion paragraph, shared links/files appendix |

---

## 📂 Grouped Inventory by Tier

### 🟣 Tier 3 — Auditable / Production System Prompts
Use these when minutes serve as an official project record, client deliverable, or automated agent system prompt requiring zero-hallucination guarantees and `[hh:mm:ss–hh:mm:ss, Speaker]` evidence citations.
1. **[`teams-transcript-crisp-records.md`](./teams-transcript-crisp-records.md)**
   - *Variant 1:* **Crisp Meeting Notes** (optimized by Microsoft Copilot) — Concise 7-section auditable schema with validation checklist.
   - *Variant 2:* **Meeting Minutes Generator — System Prompt** (optimized by Claude Opus 4.8 High) — Full XML-delimited input specification (`<metadata>`, `<transcript>`, `<chat>`), speaker alias resolution, mid-meeting reversal auditing, and worked examples.
2. **[`detailed-meeting-transcript-analysis.md`](./detailed-meeting-transcript-analysis.md)**
   - **MSTeams Meeting Transcript Analysis** (by Azure Foundry agent GPT-4o) — Enforces ISO 8601 timestamps, SMART action item numbering (`A-1`, `A-2`), and confidence levels (`High/Medium/Low`).

### 🔵 Tier 2 — Action-Prioritized & Specialized Prompts
Use these for internal engineering syncs, project management tracking, stakeholder sentiment checks, and follow-up drafting.
3. **[`analyse-msteams-transcript.md`](./analyse-msteams-transcript.md)**
   - *Variant 1:* **Objective Summarizer with Prioritized Action Table** (Gemini 1.5 Pro) — Surfaces a `Priority | Action Item | Owner | Due Date | Source` Markdown table right below the Executive Summary.
   - *Variant 2:* **Comprehensive MS Teams Call Notes: Agenda-Based Summary and Follow-Up Planner** — Detailed 7-section agenda breakdown with `[Explicit]` vs. `[Implicit]` action tagging and long-transcript sectioning instructions.
4. **[`meeting-transcript-analysis-prompt.md`](./meeting-transcript-analysis-prompt.md)**
   - Extracts Summary, Decisions, Action Items, Open Questions/Risks, Stakeholders/Mentions, **Participant Tone & Team Dynamics** (collaborative, defensive, formal, etc. with direct quotes), and a **Suggested Follow-up Email / Teams Post**.
5. **[`summarise-msteams-meeting.md`](./summarise-msteams-meeting.md)**
   - *Variant 1:* **MS Teams Comprehensive Minutes** with explicit/implicit action wrap-up and chat highlights.
   - *Variant 2:* **MS Teams Chat Transcript 7-Question Extractor** (milestones, new members, challenges, pending tasks, client feedback, technical issues, deadlines).
6. **[`detailed-meeting-minutes.md`](./detailed-meeting-minutes.md)** & **[`comprehensive-summary.md`](./comprehensive-summary.md)**
   - Lightweight structured checklists covering Meeting Title, Date/Time, Agenda Items, Action Items, Next Steps, Chat Highlights / Speakers, and Accuracy/Clarity guidelines.

### 🟢 Tier 1 — Quick & Lightweight Summaries
7. **[`summarise-meeting-transcript.md`](./summarise-meeting-transcript.md)**
   - 4-point prompt producing an introduction paragraph, bulleted topics/decisions, concluding outcome paragraph, and an appendix of shared links/files.

---

## 🔗 Related Categories

- [`../chat-analysis/`](../chat-analysis/) — Asynchronous chat & client thread question-answering prompts.
- [`../task-management/`](../task-management/) & [`../office365-copilot/`](../office365-copilot/) — Extracting action checklists from emails and workspace threads.
- [`../training-and-learning/`](../training-and-learning/) — Summarizing recorded technical classes and educational sessions (rather than operational meetings).

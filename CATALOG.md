# Master Prompt & Use-Case Catalog

A single-page searchable index of every prompt, system instruction, and AI use case in this repository, organized by **Functional Domain** and **Tier** (`🟢 Quick`, `🔵 Structured`, `🟣 System`).

> [!TIP]
> See [`STANDARDS.md`](./STANDARDS.md) for the classification model and [`templates/`](./templates/) to add new entries.

---

## ⚡ Quick-Pick Decision Guide ("I need to...")

| I want to... | Recommended Prompt | Tier | Alternative / Variant |
| :--- | :--- | :--- | :--- |
| **Produce auditable MS Teams minutes with `[hh:mm:ss]` citations** | [`meetings/teams-transcript-crisp-records.md`](./meetings/teams-transcript-crisp-records.md) | `🟣 System` | [`meetings/detailed-meeting-transcript-analysis.md`](./meetings/detailed-meeting-transcript-analysis.md) |
| **Extract a prioritized action-item table from a meeting** | [`meetings/analyse-msteams-transcript.md`](./meetings/analyse-msteams-transcript.md) | `🔵 Structured` | [`meetings/summarise-msteams-meeting.md`](./meetings/summarise-msteams-meeting.md) |
| **Analyze meeting tone/dynamics & draft a follow-up email** | [`meetings/meeting-transcript-analysis-prompt.md`](./meetings/meeting-transcript-analysis-prompt.md) | `🔵 Structured` | [`meetings/detailed-meeting-minutes.md`](./meetings/detailed-meeting-minutes.md) |
| **Get a quick 3-paragraph meeting recap** | [`meetings/summarise-meeting-transcript.md`](./meetings/summarise-meeting-transcript.md) | `🟢 Quick` | [`meetings/comprehensive-summary.md`](./meetings/comprehensive-summary.md) |
| **Write a clean Git commit message from `git diff`** | [`software-development-lifecycle/create-git-commit-messages.md`](./software-development-lifecycle/create-git-commit-messages.md) | `🔵 Structured` | [`software-development-lifecycle/git-ops.md`](./software-development-lifecycle/git-ops.md) (<40 words) |
| **Summarize commits into a Bitbucket Pull Request** | [`software-development-lifecycle/create-bitbucket-pull-requests.md`](./software-development-lifecycle/create-bitbucket-pull-requests.md) | `🟢 Quick` | — |
| **Debug a failing or slow Bitbucket CI/CD pipeline log** | [`software-development-lifecycle/debug-bitbucket-pipeline.md`](./software-development-lifecycle/debug-bitbucket-pipeline.md) | `🔵 Structured` | [`troubleshooting-debugging/readme.md`](./troubleshooting-debugging/readme.md) |
| **Audit multi-format files/logs for a service migration** | [`software-development-lifecycle/service-migration-analysis-prompts.md`](./software-development-lifecycle/service-migration-analysis-prompts.md) | `🔵 Structured` | — |
| **Run a deep monthly reflection on daily Markdown worklogs** | [`retrospectives/worklog-monthly-reflection.md`](./retrospectives/worklog-monthly-reflection.md) | `🟣 System` | [`retrospectives/monthly-worklog-analysis.md`](./retrospectives/monthly-worklog-analysis.md) (with 7 Mermaid charts) |
| **Run an end-of-week engineering / GTD retrospective** | [`retrospectives/weekly-retro.md`](./retrospectives/weekly-retro.md) | `🔵 Structured` | [`retrospectives/readme.md`](./retrospectives/readme.md) |
| **Audit an AI chat session & create a context hand-off prompt** | [`ai-use-cases/extract-ai-chat-achievements-todos.md`](./ai-use-cases/extract-ai-chat-achievements-todos.md) | `🟣 System` | — |
| **Extract a prioritized task checklist from recent emails** | [`office365-copilot/extract-tasks-from-emails.md`](./office365-copilot/extract-tasks-from-emails.md) (10d) | `🟢 Quick` | [`task-management/todos-extraction.md`](./task-management/todos-extraction.md) (YTD) |
| **Summarize a technical training class or video transcript** | [`training-and-learning/assess-class-training-transcript.md`](./training-and-learning/assess-class-training-transcript.md) | `🔵 Structured` | [`training-and-learning/prompts-transcript-training-videos.md`](./training-and-learning/prompts-transcript-training-videos.md) |
| **Extract structured data & action items from a Confluence PDF** | [`pdfs/pdf-ops.md`](./pdfs/pdf-ops.md) | `🔵 Structured` | [`ai-use-cases/readme.md`](./ai-use-cases/readme.md) |
| **Review and assess a privacy policy** | [`policies/concise-summary.md`](./policies/concise-summary.md) | `🟢 Quick` | [`policies/summarise-privacy-policy.md`](./policies/summarise-privacy-policy.md) |
| **Summarize an online article or general video script** | [`content-summarization/summarise-online-articles.md`](./content-summarization/summarise-online-articles.md) | `🟢 Quick` | [`content-summarization/summarise-video-script.md`](./content-summarization/summarise-video-script.md) |

---

## 1. Engineering, SDLC & Operations

Directories: [`software-development-lifecycle/`](./software-development-lifecycle/) · [`troubleshooting-debugging/`](./troubleshooting-debugging/)

| File | Prompt / Asset Name | Tier | Input | Output | Notes / Platform |
| :--- | :--- | :--- | :--- | :--- | :--- |
| [`software-development-lifecycle/create-git-commit-messages.md`](./software-development-lifecycle/create-git-commit-messages.md) | General & SDLC Git Commit Messages (3 variants) + Jira `D09-` Commit Extractors (3 variants) | `🔵 Structured` / `🟢 Quick` | `git diff` | 50/72-rule commit message (<75w or <140–150w with `D09-` Jira IDs & XML exclusion) | Any LLM |
| [`software-development-lifecycle/git-ops.md`](./software-development-lifecycle/git-ops.md) | Ultra-Concise Git Commit Generator (<40 words) | `🟢 Quick` | `git diff` | Imperative title + intent summary (<40 words) | Any LLM |
| [`software-development-lifecycle/create-bitbucket-pull-requests.md`](./software-development-lifecycle/create-bitbucket-pull-requests.md) | Bitbucket Pull Request Executive Summary | `🟢 Quick` | Git commit messages / diff | PR executive summary | Bitbucket / Any LLM |
| [`software-development-lifecycle/debug-bitbucket-pipeline.md`](./software-development-lifecycle/debug-bitbucket-pipeline.md) | Bitbucket Pipeline Execution Log Analyzer | `🔵 Structured` | CI/CD pipeline log (`.txt`) | 8-part diagnostic report (status, steps, errors, perf, bottlenecks, fixes) | Any LLM |
| [`software-development-lifecycle/service-migration-analysis-prompts.md`](./software-development-lifecycle/service-migration-analysis-prompts.md) | Service Migration Lift & Shift Multi-File Analyzer | `🔵 Structured` | Directory of `.docx`, `.txt`, `.json`, `.xml`, `.html`, `.pdf` | Consolidated migration report, timeline, stakeholders, log vs. meeting discrepancies | EFTPOS / Enterprise Ops |
| [`troubleshooting-debugging/readme.md`](./troubleshooting-debugging/readme.md) | Troubleshooting & Debugging Index & Diagnostic Framework | `🔵 Structured` | Logs, stack traces, pipeline outputs | Root-cause analysis & remediation checklist | Cross-domain hub |

---

## 2. Meetings, Collaboration & Communications

Directories: [`meetings/`](./meetings/) · [`chat-analysis/`](./chat-analysis/)

| File | Prompt / Asset Name | Tier | Input | Output | Notes / Platform |
| :--- | :--- | :--- | :--- | :--- | :--- |
| [`meetings/teams-transcript-crisp-records.md`](./meetings/teams-transcript-crisp-records.md) | Crisp Meeting Notes & System Prompt (2 variants) | `🟣 System` | `<metadata>`, `<transcript>`, `<chat>` | Auditable 7-section minutes with `[hh:mm:ss, Speaker]` evidence, ISO 8601, alias normalization, confidence levels | M365 Copilot / Claude Opus 4.8 High |
| [`meetings/detailed-meeting-transcript-analysis.md`](./meetings/detailed-meeting-transcript-analysis.md) | Auditable MS Teams Transcript Analyzer | `🟣 System` | MS Teams transcript | 7-section minutes with SMART action IDs (`A-1`), timestamps, confidence levels, sparse-data fallback | Azure AI Foundry GPT-4o |
| [`meetings/analyse-msteams-transcript.md`](./meetings/analyse-msteams-transcript.md) | Action-Prioritized Summarizer & Agenda-Based Planner (2 variants) | `🔵 Structured` | MS Teams transcript | Executive summary + Markdown priority table (`High/Med/Low`) + agenda topics + strategic wrap-up | Gemini 1.5 Pro / Any LLM |
| [`meetings/meeting-transcript-analysis-prompt.md`](./meetings/meeting-transcript-analysis-prompt.md) | Meeting Analyzer with Tone Dynamics & Follow-Up Draft | `🔵 Structured` | Raw meeting transcript file | Summary, decisions, actions, risks, stakeholder mentions, **participant tone shift analysis**, draft follow-up post/email | Any LLM |
| [`meetings/summarise-msteams-meeting.md`](./meetings/summarise-msteams-meeting.md) | MS Teams Meeting Minutes + MS Teams Chat Transcript Q&A (2 variants) | `🔵 Structured` / `🟢 Quick` | MS Teams call or chat transcript | Comprehensive meeting notes OR 7-question project chat milestone/issue extraction | MS Teams / Any LLM |
| [`meetings/comprehensive-summary.md`](./meetings/comprehensive-summary.md) | Comprehensive Meeting Transcript Summary | `🔵 Structured` | Meeting transcript | Title, Date/Time, Agenda Items, Action Items, Next Steps, Other Notes, Speakers & Roles | Any LLM |
| [`meetings/detailed-meeting-minutes.md`](./meetings/detailed-meeting-minutes.md) | Detailed Meeting Minutes (with Chat Highlights & Attendance Ratio) | `🔵 Structured` | Meeting transcript | Standard minutes + Chat Highlights + Attended vs. Invited headcount | Any LLM |
| [`meetings/summarise-meeting-transcript.md`](./meetings/summarise-meeting-transcript.md) | Quick 4-Part Meeting Transcript Summary | `🟢 Quick` | Meeting text transcript | Intro paragraph, bulleted topics/decisions, concluding paragraph, shared links/files appendix | Any LLM |
| [`chat-analysis/chat-transcription.md`](./chat-analysis/chat-transcription.md) | Client Project Chat Transcript 7-Question Extractor | `🟢 Quick` | Project chat log | Milestones, new team members/roles, challenges, pending actions, client feedback, tech issues, deadlines | Any LLM |

---

## 3. Productivity, Task Management & Retrospectives

Directories: [`retrospectives/`](./retrospectives/) · [`task-management/`](./task-management/) · [`office365-copilot/`](./office365-copilot/)

| File | Prompt / Asset Name | Tier | Input | Output | Notes / Platform |
| :--- | :--- | :--- | :--- | :--- | :--- |
| [`retrospectives/worklog-monthly-reflection.md`](./retrospectives/worklog-monthly-reflection.md) | Monthly Worklog Analyst — 10-Section System Prompt | `🟣 System` | Consolidated daily Markdown worklogs (`GOALS`, `MORNING`, `WRAP UP`, `Timesheet` WBS) | 10 `<fieldset>` prose sections: Executive Summary, Themes, Goal Calibration, Open Loops, Wins, WBS Alignment, Frameworks (Deep Work/GTD/PARA), Next Month Focus | Claude Sonnet 4.6 / Antigravity |
| [`retrospectives/monthly-worklog-analysis.md`](./retrospectives/monthly-worklog-analysis.md) | Master Prompt for Markdown Worklog Analysis (2 variants: Visual + Verbose) | `🔵 Structured` | Consolidated daily Markdown worklogs | 6-section reflection + **7 Mermaid diagrams** visualizing patterns (Variant 1) or formatted prose/bullets (Variant 2) | Any LLM |
| [`retrospectives/weekly-retro.md`](./retrospectives/weekly-retro.md) | Weekly Engineering & GTD Retrospective Prompt | `🔵 Structured` | 5-day Markdown worklog slice (`Monday–Friday`) | Weekly accomplishments, carry-over stalls, blocker patterns, WBS check, and Monday Top-3 kickoff plan | Any LLM |
| [`retrospectives/readme.md`](./retrospectives/readme.md) | Retrospectives Overview & Terminology Guide | `🟢 Quick` | — | Definitions of Weekly Retrospective, Weekly Review (GTD), and Reflective Practice + category index | Reference |
| [`office365-copilot/extract-tasks-from-emails.md`](./office365-copilot/extract-tasks-from-emails.md) | 10-Day Email Action Checklist Extractor | `🟢 Quick` | Last 10 days of Outlook emails | Checklist grouped by action owner, ordered by priority and end date | M365 Copilot (Premium) |
| [`office365-copilot/readme.md`](./office365-copilot/readme.md) | Microsoft 365 Copilot Prompt Index | `🟢 Quick` | — | M365 Copilot license context and prompt catalog | M365 Copilot |
| [`task-management/todos-extraction.md`](./task-management/todos-extraction.md) | Year-to-Date Email Action Checklist Extractor | `🟢 Quick` | Emails from current year | Checklist against action owners ordered by priority and end date | M365 Copilot / Email AI |

---

## 4. Content, Document & Learning Intelligence

Directories: [`content-summarization/`](./content-summarization/) · [`pdfs/`](./pdfs/) · [`policies/`](./policies/) · [`training-and-learning/`](./training-and-learning/)

| File | Prompt / Asset Name | Tier | Input | Output | Notes / Platform |
| :--- | :--- | :--- | :--- | :--- | :--- |
| [`content-summarization/summarise-online-articles.md`](./content-summarization/summarise-online-articles.md) | Paragraph-by-Paragraph Online Article Summarizer | `🟢 Quick` | Article text | Numbered list with a summary of each paragraph | Any LLM |
| [`content-summarization/summarise-video-script.md`](./content-summarization/summarise-video-script.md) | Actionable Video Script Summarizer | `🔵 Structured` | Video script | Introduction, detailed main ideas, key takeaways, and "What's Next" actionable items | Azure-created / Any LLM |
| [`pdfs/pdf-ops.md`](./pdfs/pdf-ops.md) | Structured PDF & Confluence Export Intelligence Summarizer | `🔵 Structured` | Technical PDF (Confluence export with tables/code/diagrams) | Title, <200w summary, logical sections, JSON/Markdown tables, action items, clarification questions | Any LLM |
| [`policies/concise-summary.md`](./policies/concise-summary.md) | Privacy Policy Summarizer & Trust Assessor (Collapsible) | `🟢 Quick` | Privacy policy text | Data lifecycle evaluation (collection, use, storage, sharing, protection), clarity/ambiguity review, final bulleted key details | Any LLM |
| [`policies/summarise-privacy-policy.md`](./policies/summarise-privacy-policy.md) | Privacy Policy Summarizer & Trust Assessor (Direct) | `🟢 Quick` | Privacy policy text | Concise summary + transparency evaluation + improvement suggestions + bulleted key details | Any LLM |
| [`training-and-learning/assess-class-training-transcript.md`](./training-and-learning/assess-class-training-transcript.md) | Comprehensive Technical Training Session Summary | `🔵 Structured` | Recorded software engineering class transcript | 8-section summary: Executive Summary, Overview, Key Concepts, 5–8 Takeaways, Code Demos, Tools, 4–6 Next Steps, Resources | Any LLM |
| [`training-and-learning/prompts-transcript-training-videos.md`](./training-and-learning/prompts-transcript-training-videos.md) | Progressive Training Video Prompt Suite (Quick → Comprehensive) | `🔵 Structured` | Video class script / transcript | Combines quick education summary, structured video takeaways, and full 8-section technical educator summary | AWS Bedrock Claude |

---

## 5. AI Strategy, Session Ops & Use Cases

Directory: [`ai-use-cases/`](./ai-use-cases/)

| File | Prompt / Asset Name | Tier | Input | Output | Notes / Platform |
| :--- | :--- | :--- | :--- | :--- | :--- |
| [`ai-use-cases/extract-ai-chat-achievements-todos.md`](./ai-use-cases/extract-ai-chat-achievements-todos.md) | Universal AI Session Audit & Context Hand-Off Prompt | `🟣 System` | Entire AI chat session history / transcript | Executive summary, numbered achievements, `[Explicit]` vs `[Implicit]` backlog table, blind-spot analysis, and **ready-to-paste context hand-off block** | Gemini / Claude / Any LLM |
| [`ai-use-cases/readme.md`](./ai-use-cases/readme.md) | High-Level GenAI Use-Case Catalog (8 Blueprints) | `🔵 Structured` | Multimodal (images, diagrams, PDFs, forms, specs, copy) | 8 structured use cases (Batch Image Renaming, Diagram Analysis, Long-Doc Summary, Spec-to-Code, Form Extraction, Domain Assistant, Test/Fuzz Generation, Localization) + ethical/operational guardrails | Architecture Reference |

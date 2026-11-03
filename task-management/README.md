# Task Management & Action Extraction

> **Domain:** 3. Productivity, Task Management & Retrospectives | **Parent Catalog:** [`../CATALOG.md`](../CATALOG.md)

Prompts for extracting prioritized action checklists, owners, and due dates from emails, meetings, worklogs, and AI sessions.

---

## ⚡ Quick-Pick Decision Matrix (Across Email, Meetings & Sessions)

| Source Channel | Prompt File | Tier | Time Horizon / Scope |
| :--- | :--- | :--- | :--- |
| **Emails (Year-to-Date Sweep)** | [`todos-extraction.md`](./todos-extraction.md) | `🟢 Quick` | Current calendar year emails → Checklist by action owner, priority, and end date |
| **Emails (Past 10 Days Rolling)** | [`../office365-copilot/extract-tasks-from-emails.md`](../office365-copilot/extract-tasks-from-emails.md) | `🟢 Quick` | Last 10 days of Outlook emails via M365 Copilot → Checklist by owner, priority, and end date |
| **MS Teams Meeting Transcripts** | [`../meetings/analyse-msteams-transcript.md`](../meetings/analyse-msteams-transcript.md) | `🔵 Structured` | Meeting transcript → Markdown table (`Priority \| Action Item \| Owner \| Due Date \| Source`) |
| **Daily / Monthly Markdown Worklogs** | [`../retrospectives/worklog-monthly-reflection.md`](../retrospectives/worklog-monthly-reflection.md) | `🟣 System` | Daily worklogs → Stalled carry-overs, unanswered `QUESTIONS`, and next-month Top-3 kickoff list |
| **AI Chat Sessions** | [`../ai-use-cases/extract-ai-chat-achievements-todos.md`](../ai-use-cases/extract-ai-chat-achievements-todos.md) | `🟣 System` | AI conversation thread → `[Explicit]` vs. `[Implicit]` prioritized backlog table + context hand-off |

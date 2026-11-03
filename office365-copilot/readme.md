# Prompts when Copilot for Microsoft 365 License

> **Domain:** 3. Productivity, Task Management & Retrospectives | **Category:** `office365-copilot` | **Parent Catalog:** [`../CATALOG.md`](../CATALOG.md)

tested with premium license.

---

## ⚡ Microsoft 365 Copilot & MS Teams Prompt Index

Prompts in this directory and across the repository that leverage Microsoft Graph context (Outlook emails, MS Teams chats, and meeting transcripts):

| File | Tier | M365 Surface | Purpose |
| :--- | :--- | :--- | :--- |
| **[`extract-tasks-from-emails.md`](./extract-tasks-from-emails.md)** | `🟢 Quick` | Teams / Outlook Copilot | Scans emails from the **past 10 days** and builds a checklist against action owners ordered by priority and end date |
| **[`../task-management/todos-extraction.md`](../task-management/todos-extraction.md)** | `🟢 Quick` | Teams / Outlook Copilot | Scans emails from **this year** and builds a checklist against action owners ordered by priority and end date |
| **[`../meetings/teams-transcript-crisp-records.md`](../meetings/teams-transcript-crisp-records.md)** | `🟣 System` | MS Teams Copilot | *Crisp meeting Notes optimised by Copilot* — transforms a Teams transcript + chat into 7-section auditable minutes with `[hh:mm:ss, Speaker]` citations |
| **[`../meetings/summarise-msteams-meeting.md`](../meetings/summarise-msteams-meeting.md)** | `🔵 Structured` | MS Teams Copilot | Summarizes MS Teams call transcripts and 7-question project chat threads |

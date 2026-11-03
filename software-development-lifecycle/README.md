# Software Development Lifecycle (SDLC) Prompts

> **Domain:** 1. Engineering, SDLC & Operations | **Parent Catalog:** [`../CATALOG.md`](../CATALOG.md)

Prompts supporting day-to-day software engineering workflows across version control (Git commits), code review (Bitbucket Pull Requests), CI/CD pipeline diagnostics, and multi-document service migration analysis.

---

## ⚡ Quick-Pick Decision Matrix

| Goal | Recommended File | Specific Prompt / Section | Tier | Output Constraints |
| :--- | :--- | :--- | :--- | :--- |
| **Standard 50/72 Git commit from `git diff`** | [`create-git-commit-messages.md`](./create-git-commit-messages.md) | *General / SDLC git commit message* | `🔵 Structured` | Imperative subject (≤50 chars) + numbered body (≤72 chars/line, <75 words total) |
| **Ultra-short Git commit (<40 words)** | [`git-ops.md`](./git-ops.md) | *Generate a git commit message max 40 words* | `🟢 Quick` | Concise title + intent summary (≤40 words, no file paths unless needed) |
| **Git commit with Jira ID (`D09-*`) extraction** | [`create-git-commit-messages.md`](./create-git-commit-messages.md) | *using Jira* (3 variants) | `🟢 Quick` | Numbered changes + `D09-` Jira IDs on last line (optional XML file exclusion & 140–150w caps) |
| **Executive summary for a Bitbucket Pull Request** | [`create-bitbucket-pull-requests.md`](./create-bitbucket-pull-requests.md) | *Git commit summary based on git diff* | `🟢 Quick` | PR executive summary from commit history |
| **Analyze & optimize a Bitbucket CI/CD pipeline log** | [`debug-bitbucket-pipeline.md`](./debug-bitbucket-pipeline.md) | *Debugging Bitbucket* | `🔵 Structured` | 8-point assessment: status, steps, errors, perf metrics, resources, bottlenecks, improvements, anomalies |
| **Audit mixed docs/logs for a service migration** | [`service-migration-analysis-prompts.md`](./service-migration-analysis-prompts.md) | *Analyse a directory with files and notes for a service migration lift & shift* | `🔵 Structured` | Consolidated report across `.docx`, `.txt`, `.json`, `.xml`, `.html`, `.pdf` with timeline & log discrepancies |

---

## 📂 Grouped Prompt Inventory

### 1. Version Control & Code Review (Git & Bitbucket)
- **[`create-git-commit-messages.md`](./create-git-commit-messages.md)** — Master collection of 6 Git commit prompt variants:
  - *General / SDLC Commit Message (50/72 Rule)*: Enforces imperative mood, ≤50-char subject, blank separator line, and ≤72-char wrapped body under 75 words.
  - *Conversational 50/72 Variant*: Natural-language instruction for 8–12 word subject and 50–75 word total commit.
  - *Jira (`D09-`) Variants (3 options)*: Automatically extracts `D09-*` ticket keys to the final line, with options to cap at 140–150 words / 3 bullets or exclude noisy config files (`EnvironmentVariables.xml`).
- **[`git-ops.md`](./git-ops.md)** — Lightweight commit prompt focused strictly on intent over line-by-line diffs with a hard **40-word maximum**.
- **[`create-bitbucket-pull-requests.md`](./create-bitbucket-pull-requests.md)** — Generates a high-level executive summary for a Bitbucket Pull Request from a list of commit messages.

### 2. CI/CD & Operational Diagnostics
- **[`debug-bitbucket-pipeline.md`](./debug-bitbucket-pipeline.md)** — Deep-dive analyzer for attached Bitbucket Pipeline text logs covering step outcomes, errors/warnings, execution times, resource usage, and optimization opportunities.
- **[`service-migration-analysis-prompts.md`](./service-migration-analysis-prompts.md)** — Multi-artifact lift-and-shift analysis prompt (originally tailored for EFTPOS service migrations) that cross-references meeting transcripts (`.docx`) against system logs (`.txt`, `.json`, `.xml`, `.html`, `.pdf`) to flag discrepancies and build a stakeholder timeline.

---

## 🔗 Related Categories

- [`../troubleshooting-debugging/`](../troubleshooting-debugging/) — General diagnostic workflows and root-cause analysis templates.
- [`../ai-use-cases/`](../ai-use-cases/) — High-level SDLC GenAI blueprints (*Generate code from specs*, *Test-case generation & fuzzing*, *Universal AI Session Audit & Hand-Off*).

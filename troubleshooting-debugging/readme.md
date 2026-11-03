# Debugging guides, diagnostics, common issues

> **Domain:** 1. Engineering, SDLC & Operations | **Category:** `troubleshooting-debugging` | **Parent Catalog:** [`../CATALOG.md`](../CATALOG.md)

Central hub for troubleshooting, log analysis, CI/CD pipeline diagnostics, and cross-artifact discrepancy detection across engineering and operations workflows.

---

## ⚡ Diagnostic & Debugging Prompts Across the Repository

| Scenario | Prompt File | Tier | Input → Output |
| :--- | :--- | :--- | :--- |
| **CI/CD Pipeline Failure or Bottleneck** | [`../software-development-lifecycle/debug-bitbucket-pipeline.md`](../software-development-lifecycle/debug-bitbucket-pipeline.md) | `🔵 Structured` | Bitbucket pipeline `.txt` log → 8-point report (status, failed steps, errors, timings, bottlenecks, remediation) |
| **Log vs. Meeting Note Discrepancy (Service Migration)** | [`../software-development-lifecycle/service-migration-analysis-prompts.md`](../software-development-lifecycle/service-migration-analysis-prompts.md) | `🔵 Structured` | Directory of `.txt` logs, `.json`/`.xml` payloads, `.docx` notes → Consolidated status report & discrepancy list |
| **Audit an AI Troubleshooting Session & Hand Off Context** | [`../ai-use-cases/extract-ai-chat-achievements-todos.md`](../ai-use-cases/extract-ai-chat-achievements-todos.md) | `🟣 System` | Full troubleshooting chat thread → Resolved issues, `[Explicit]`/`[Implicit]` pending items, next-session prompt |

---

## 🛠️ Standard Root-Cause Analysis (RCA) & Log Triage Prompt

> **Domain:** 1. Engineering, SDLC & Operations | **Category:** `troubleshooting-debugging` | **Tier:** 🔵 Structured  
> **Use When:** Investigating application stack traces, cloud infrastructure errors (GCP/AWS/Azure), or runtime failures where you need a structured hypothesis-driven diagnosis before changing code or config.  
> **Input:** Error log / stack trace + environment context | **Output:** Root-cause ranking, verification commands, minimal fix, and prevention checklist

<details>
<summary>🔍 Structured Root-Cause Analysis & Triage Prompt (Click to expand & copy)</summary>

```text
Role & Persona:
You are a Senior Site Reliability Engineer (SRE) and Systems Debugger. Your objective is to analyze the provided error logs, stack traces, or configuration snippets and produce a structured, hypothesis-driven root-cause analysis and minimal-blast-radius remediation plan.

Context & Guardrails:
- Rely strictly on the provided logs and context. Do not invent configuration values or unobserved metrics.
- Prefer small-batch, reversible verification and remediation steps (DevOps mindset).
- Clearly distinguish confirmed facts in the log from inferred hypotheses (label with Confidence: High/Medium/Low).

Task Instructions:
1. **Symptom Summary:** State the exact failure mode, affected component/service, and first-failing step or timestamp.
2. **Ranked Root-Cause Hypotheses:** List the top 1–3 most likely root causes ordered by probability, citing the exact log lines that support each hypothesis.
3. **Fast Verification Steps:** Provide read-only diagnostic commands or checks to confirm or rule out each hypothesis before making changes.
4. **Minimal Remediation Plan:** Provide the smallest, safest change to resolve the issue, along with a rollback step if the change does not resolve it.
5. **Preventative Follow-Up:** Suggest 1–2 observability, test, or pipeline guardrails to prevent recurrence.
```

</details>

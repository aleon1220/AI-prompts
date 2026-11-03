# [Action-Oriented Prompt Title]

> **Domain:** [Engineering & SDLC | Meetings & Comms | Productivity & Retrospectives | Content & Document Intelligence | AI Strategy & Use Cases] | **Category:** `[folder-name]` | **Tier:** [🟢 Quick | 🔵 Structured | 🟣 System]  
> **Use When:** [1-sentence guidance on when to pick this prompt over simpler/heavier alternatives.]  
> **Input:** [e.g., Raw transcript, `git diff`, PDF export, consolidated Markdown log] | **Output:** [e.g., Prioritized Markdown table, commit block, executive summary]  
> **Target / Tested With:** [Model-agnostic (Any LLM) | M365 Copilot | Gemini | Claude | GPT-4o]

## Overview

[Optional 1–3 lines describing context, prerequisites, or CLI commands to prepare the input.]

## Prompt

<details>
<summary>📝 [Prompt Title] (Click to expand & copy)</summary>

```text
Role & Persona:
You are an expert [role/domain specialist]. Your objective is to [core objective].

Context:
[Describe the nature of the input data, common noise/edge cases, and intended audience.]

Task Instructions:
1. [Step 1]
2. [Step 2]
3. [Step 3]

Output Constraints & Guardrails:
- Zero Hallucination: Rely strictly on the provided input. Do not invent facts, names, dates, or metrics.
- Inference Labeling: Label any reasonable inference as "(Inferred)" with Confidence (High/Medium/Low).
- Tone & Format: Maintain an objective, concise tone in clean Markdown.

Output Structure:
### 1. Executive Summary
[2–4 sentences or bullets]

### 2. Core Analysis / Deliverables
[Structured sections or table]

### 3. Action Items / Next Steps
| Priority | Action Item | Owner | Due Date | Source |
| :--- | :--- | :--- | :--- | :--- |
| [High/Med/Low] | [Imperative task] | [Name or "Not specified"] | [ISO Date or "Not specified"] | `[Explicit]` / `[Implicit]` |
```

</details>

## Related Prompts

- [`../folder/example.md`](../README.md) — [Why/when you might use that prompt instead]

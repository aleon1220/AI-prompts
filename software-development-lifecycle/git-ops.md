# Generate a git commit message max 40 words

> **Domain:** 1. Engineering, SDLC & Operations | **Category:** `software-development-lifecycle` | **Tier:** 🟢 Quick  
> **Use When:** You want an ultra-concise (<40 words) intent-focused commit message without line-by-line details or file paths.  
> **Input:** `git diff` output | **Output:** Imperative title + ≤40-word commit description  
> **Target / Tested With:** Any LLM · See also [`create-git-commit-messages.md`](./create-git-commit-messages.md) for 50/72 & Jira `D09-` rules

<details>
<summary>📝 Concise Git Commit Message (Max 40 Words)</summary>

```text
Generate a concise and clear git commit message based on the following git diff. Please make it 

Requirements:
Summarize the intent of the change, not the line-by-line diff.

Use the imperative mood (e.g., “Add”, “Fix”, “Refactor”).

For a title please make a very concise title.

Maximum of 40 words the description of the git commit.

If multiple logical changes appear, group them into a single coherent summary.

Do not mention file paths unless necessary for clarity.
```

</details>

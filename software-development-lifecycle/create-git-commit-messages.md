# Git Assistance

> **Domain:** 1. Engineering, SDLC & Operations | **Category:** `software-development-lifecycle` | **Tier:** 🔵 Structured / 🟢 Quick  
> **Use When:** Generating clean, 50/72-compliant Git commit messages from `git diff` (with optional Jira `D09-*` key extraction and config file exclusions).  
> **Input:** `git diff` output | **Output:** Plain-text Git commit message (≤50-char subject + wrapped numbered body)  
> **Target / Tested With:** Any LLM · See also [`git-ops.md`](./git-ops.md) for ultra-short (<40 words) commits

during software development a commit message should be concise and give a helpful overview of the changes.
```bash
git diff | clip.exe
```

### General git commit message

* enforces a short subject plus a focused body explaining intent rather than implementation.

<details>
<summary> General git commit message 📝 </summary>

```text
Act as a software engineer. Generate a clean, concise Git commit message
based on the provided changes/diff.

Output only the commit message inside a single plain-text code block
for easy copying.

Formatting rules (strictly enforced):

1) Subject line
   - Use imperative mood (e.g., "Add", "Fix", "Update", "Refactor").
   - Capitalize first word, no ending punctuation.
   - Maximum 50 characters.
   - Summarize the primary change only.

2) Separation
   - Exactly one blank line between the subject line and the body.

3) Body structure (total body <= 75 words)
   - First line: an **executive summary** (one sentence, <= 15 words)
     that states the primary impact or rationale.
   - Follow with **up to 3 concise bullet points** (use markdown dashes `-`)
     summarizing key changes or effects. Each bullet: one short sentence,
     aim for 6–12 words.
   - Explain **what** changed and **why** — do not describe implementation details.
   - Hard wrap all lines at 72 characters.

4) Tone & style
   - Clear, factual, and terse. Avoid filler words.
   - Use active voice and present/imperative tense.
   - Do not include issue tracker metadata unless explicitly requested.

Example desired output format:

Subject line within 50 chars

Executive summary sentence (<= 15 words)

* Bullet one (concise)
* Bullet two (concise)
* Bullet three (concise)

When given a diff, produce the commit message that best follows the above rules.
```

</details>

### SDLC git concise commit message

<details>
<summary> SDLC git commit message 📝 </summary>

```text
Act as a software engineer. Generate a clean Git commit message based on the provided changes/diff. Format the output inside a single plain text code block for easy copying.

Formatting Rules:
1. Subject Line:
   - Imperative mood (e.g., "Add", "Fix", "Update", "Refactor").
   - Capitalized, no ending punctuation.
   - Maximum 50 characters (concise summary of the primary change).

2. Blank Line:
   - Exactly one blank line between the subject line and the body.

3. Body:
   - Explain the "what" and "why" behind the changes, not the "how".
   - Hard wrap all lines at 72 characters.
   - Use a markdown numbered list to summarize key changes if multiple logical updates exist.
   - Keep the entire commit message focused and under 75 words total.
```

</details>

### General git commit message
<details>
<summary> General git commit message 📝 </summary>

```text
please do me a favor and create a git commit message for the git diff below. Use a numbered list format to list the changes.
consider Subject Line: Should be a concise summary of the changes. Typically, it should be no more than 50 characters

Body:
If additional detail is necessary, the body of the commit message can be used.
Each line in the body should be wrapped at around 72 characters.
The body should explain the "what" and "why" of the changes, not the "how".

In terms of word count, the subject line might be around 8-12 words, and the body can vary, but it's recommended to keep it concise and focused. Generally, a good commit message might contain around 50-75 words in total, including both the subject and the body, if needed.
```

</details>
---

## using Jira 

<details>
<summary> git commit when using Jira ID with pattern 📝 </summary>

```text
create a git commit message for the git diff below. Use a numbered list format to list the changes.

At the end of the message extract any Jira IDs in starting with D09- and add them in the last line
```

</details>

<details>

<summary> Jira ID with pattern and exclude changes to a particular XML file 📝 </summary>

```text
create a git commit message max 140 words for the git diff below. 

Use a numbered list format to list the changes. 
Exclude the file EnvironmentVariables.xml file and changes related to it as is not committed.

At the end of the message extract any Jira IDs in starting with "D09-" and add them in the last line.
```

</details>

<details>
<summary> git commit when using Jira ID with pattern📝 </summary>

```text
create a git commit message for the git diff below. Use a numbered list format to list the changes.
At the end of the message extract any Jira IDs in starting with D09- and add them in the last line.
Max 3 bulletpoints in the description and max total of 150 words
```

</details>

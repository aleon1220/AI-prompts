# Git Assistance
during software development a commit message should be concise and give a helpful overview of the changes.
```bash
git diff | clip.exe
```
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

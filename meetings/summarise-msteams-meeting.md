# MS Teams Meeting Minutes & Project Chat Summarizer

> **Domain:** 2. Meetings, Collaboration & Communications | **Category:** `meetings` | **Tier:** 🔵 Structured / 🟢 Quick  
> **Use When:** Summarizing either a full MS Teams call transcript (with explicit/implicit action item prioritization) OR a resourceful MS Teams project chat log using 7 structured delivery questions.  
> **Input:** MS Teams call transcript or MS Teams chat transcript | **Output:** Detailed meeting minutes OR 7-question project milestone/issue breakdown  
> **Target / Tested With:** MS Teams / Any LLM · See also [`../chat-analysis/chat-transcription.md`](../chat-analysis/chat-transcription.md)

<details>
<summary> MSTeams Meetings transcript comprehensive prompt minutes 👨‍💻 👩‍💻 💻 🖥️ 📊 📈 💡 📢</summary>

```text
Please generate detailed meeting notes and summary. 

Include the following elements in your output:

- Meeting Title: Provide the title or a concise description of the meeting's purpose.
- Date and Time: Clearly indicate the date and time the meeting took place.
- Agenda Items: Organize the meeting minutes based on the agenda items discussed. Clearly identify each agenda item and summarize the key points, discussions, and decisions related to it.
- Action Items:  Identify and list any specific action items that emerged from the meeting. For each action item, specify the person responsible for completing it and the deadline, if mentioned.
- Next Steps:  If there were any discussions or decisions about the next steps to be taken after the meeting, summarize them concisely.

Important Considerations:

- you are using a transcript from a MSTeams call
- Accuracy: Ensure that your summary accurately reflects the discussions and decisions made in the transcript.
- Conciseness: Aim to be concise and focused in your summary while capturing all the essential information.
- Clarity:  Use clear and straightforward language to present the information in an easily understandable manner.
- Objectivity: Maintain an objective and neutral tone throughout the summary.

Additional Tips:

- If the transcript is long, consider breaking it down into smaller sections to make the summarization process more manageable.
- Use bullet points and numbered lists to organize information for better readability.
- Proofread your summary carefully to eliminate any errors or inconsistencies.

Wrap up section:
Add a section that makes emphasis on action items explicitly and implicitly mentioned. Suggest next steps and prioritise

Appendix section Chat Highlights:
- Other Notes:  Include any additional information or important details that were discussed during the meeting but don't fit into the above categories.
- Attendees: if names are mentioned, list meeting participants, identify their roles or affiliations.
```
</details>

---

<details>
<summary>
MSTeams Chat transcript 
</summary>

```text
Please summarise the attached transcript using the best patterns for summaries that you know.

Considerations
> cases where the chat contains resourceful information

1. What are the key milestones achieved in the project for the client?

2. Who are the new team members that joined the project, and what roles do they play?

3. What were the main challenges faced during the project, and how were they resolved?

4. What are the pending action items or tasks that need to be addressed?

5. What feedback or updates have been provided by the client regarding the project's progress?

6. What are the significant technical issues encountered, and what solutions were implemented?

7. What are the upcoming project deadlines or important events that the team should be aware of?
```
</details>

# Detailed Meeting Minutes (with Chat Highlights & Attendance Ratio)

> **Domain:** 2. Meetings, Collaboration & Communications | **Category:** `meetings` | **Tier:** 🔵 Structured  
> **Use When:** Generating standard meeting minutes that also capture Chat Highlights and Attended vs. Invited headcount.  
> **Input:** Meeting transcript + invite/chat metadata | **Output:** Detailed minutes (Title, Date/Time, Agenda, Actions, Next Steps, Chat Highlights, Notes, Attendance count)  
> **Target / Tested With:** Any LLM · Compare with [`comprehensive-summary.md`](./comprehensive-summary.md)

<details>
<summary>📝 Detailed Meeting Minutes Prompt (with Chat & Attendance Ratio)</summary>

```text
Please generate detailed meeting minutes. Include the following elements in your output:

* Meeting Title: Provide the title or a concise description of the meeting's purpose.
* Date and Time: Clearly indicate the date and time the meeting took place.
* Agenda Items: Organize the meeting minutes based on the agenda items discussed. Clearly identify each agenda item and summarize the key points, discussions, and decisions related to it.
* Action Items:  Identify and list any specific action items that emerged from the meeting. For each action item, specify the person responsible for completing it and the deadline, if mentioned.
* Next Steps:  If there were any discussions or decisions about the next steps to be taken after the meeting, summarize them concisely.
* Chat Highlights: 
* Other Notes:  Include any additional information or important details that were discussed during the meeting but don't fit into the above categories.
* Attendees: if available List the total number of people that attended the meeting vs the total number of people invited.

Important Considerations:

* Accuracy: Ensure that your summary accurately reflects the discussions and decisions made in the transcript.
* Conciseness: Aim to be concise and focused in your summary while capturing all the essential information.
* Clarity:  Use clear and straightforward language to present the information in an easily understandable manner.
* Objectivity: Maintain an objective and neutral tone throughout the summary.

Additional Tips:

* If the transcript is long, consider breaking it down into smaller sections to make the summarization process more manageable.
* Use bullet points and numbered lists to organize information for better readability.

* Proofread your summary carefully to eliminate any errors or inconsistencies.
```

</details>

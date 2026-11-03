# prompt to generate a comprehensive summary for a meeting transcript

> **Domain:** 2. Meetings, Collaboration & Communications | **Category:** `meetings` | **Tier:** 🔵 Structured  
> **Use When:** Generating standard, readable meeting minutes with explicit speaker/role identification when mentioned in the transcript.  
> **Input:** Meeting transcript | **Output:** Structured minutes (Title, Date/Time, Agenda, Actions, Next Steps, Notes, Speakers)  
> **Target / Tested With:** Any LLM · Compare with [`detailed-meeting-minutes.md`](./detailed-meeting-minutes.md) (adds Chat & Attendance ratio)

<details>
<summary> comprehensive summary for a meeting transcript 📅📝🧑‍💼🧑‍💻📈 </summary>

```text
Please generate detailed meeting minutes. Include the following elements in your output:

* Meeting Title: Provide the title or a concise description of the meeting's purpose.
* Date and Time: Clearly indicate the date and time the meeting took place.
* Agenda Items: Organize the meeting minutes based on the agenda items discussed. Clearly identify each agenda item and summarize the key points, discussions, and decisions related to it.
* Action Items:  Identify and list any specific action items that emerged from the meeting. For each action item, specify the person responsible for completing it and the deadline, if mentioned.
* Next Steps:  If there were any discussions or decisions about the next steps to be taken after the meeting, summarize them concisely.
* Other Notes:  Include any additional information or important details that were discussed during the meeting but don't fit into the above categories.

* Speakers from Attendees: List meeting participants, identify their roles or affiliations. Only if speaker mentions them.

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

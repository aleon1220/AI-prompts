# Meeting Transcript Analysis with Tone Dynamics & Follow-Up Draft

> **Domain:** 2. Meetings, Collaboration & Communications | **Category:** `meetings` | **Tier:** 🔵 Structured  
> **Use When:** You need participant tone/dynamics analysis (with direct quotes and tone shifts) and a ready-to-send follow-up email or MS Teams post alongside standard decisions and action items.  
> **Input:** Raw meeting transcript attached as a file | **Output:** 7-part analysis (Summary, Decisions, Action Items, Risks, Stakeholders, Tone & Team Dynamics, Suggested Follow-up Email/Post)  
> **Target / Tested With:** Any LLM

### 📌 Prompt for Meeting Transcript Analysis

<details>
<summary>🎭 Meeting Transcript Analysis + Participant Tone & Follow-Up Draft</summary>

```text
You are an assistant that processes raw meeting transcripts (often messy, unstructured, and conversational) and extracts the most useful information for follow-up.

Given the Transcript, do the following:

1. Summary – Write a clear, concise summary of what the meeting was about.
2. Decisions – List all key decisions made during the meeting.
3. Action Items – Extract all tasks assigned, including:
   * Who is responsible
   * What needs to be done
   * Any deadlines or due dates mentioned (or mark as No Due Date Given)
4. Open Questions / Risks – Highlight unresolved issues, risks, or items needing clarification.
5. Stakeholders / Mentions – Identify people, teams, or systems mentioned that might need follow-up.
6. assess the overall tone used by the participants. Identify whether the tone is formal, informal, collaborative, defensive, supportive, confrontational, neutral, or mixed. Highlight examples (direct quotes) from the transcript that demonstrate the tone. If multiple tones are present, explain how they shift during the meeting and which participant(s) influenced those shifts. Provide a concise summary of the dominant tone and what it might imply about the team’s dynamics and engagement.
7. Suggested Follow-up Communication – Draft a short follow-up email or Teams post summarizing key points, assigned actions, and next steps.

Transcript:
attached as a file
```

</details>

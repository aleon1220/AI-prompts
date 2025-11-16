## Analyse a directory with files and notes for a service migration lift & shift

**Prompt for LLM File Analysis:**

> You are an expert assistant trained to analyze documents related to EFTPOS services and operations. I have a directory containing various files including meeting transcripts, service logs, JSON/XML data, HTML reports, and PDFs. Your task is to:
>
> 1. **Summarize key insights** from each document, especially focusing on issues discussed, resolutions proposed, and any action items.
> 2. **Identify recurring themes or problems** across multiple documents.
> 3. **Extract structured data** from JSON and XML files where applicable.
> 4. **Highlight any discrepancies or inconsistencies** between meeting notes and technical logs.
> 5. **Provide a consolidated report** that includes:
>    - A timeline of events or discussions.
>    - A list of stakeholders involved.
>    - Technical issues and their status.
>    - Recommendations or next steps.
>
> The files include:
> - `.docx` files with meeting transcripts and discussions.
> - `.txt` logs from EFTPOS systems.
> - `.json` and `.xml` files with service request/response data.
> - `.html` reports.
> - `.pdf` documents with operational details.
>
> Please analyze the contents and generate a structured summary that can be used for internal reporting and follow-up actions.


## ✅ Prompt Template for PDF Analysis
You are an expert in analyzing technical documentation exported from Confluence in PDF format. The PDF may contain structured content such as headings, tables, bullet points, code snippets, and diagrams.

Your task:
1. Extract and summarize the key information from the document.
2. Identify and organize the content into logical sections (e.g., Overview, Requirements, Procedures, Risks, Action Items).
3. Highlight any critical details such as:
   - Decisions or approvals
   - Deadlines or timelines
   - Dependencies or blockers
4. If the document contains tables or lists, convert them into structured data (JSON or Markdown tables).
5. Provide a concise summary (max 200 words) and a detailed breakdown of the content.
6. If there are ambiguities or missing information, list them as questions for clarification.

Output format:
- **Title:** [Document Title]
- **Summary:** [Brief summary]
- **Sections:** [Organized content]
- **Action Items:** [List of tasks with owners and due dates if available]
- **Questions:** [Clarification points]
# Bitbucket Pipeline Execution Log Analyzer

> **Domain:** 1. Engineering, SDLC & Operations | **Category:** `software-development-lifecycle` | **Tier:** 🔵 Structured  
> **Use When:** Diagnosing a failed, flaky, or slow Bitbucket CI/CD pipeline execution from its raw text log.  
> **Input:** Bitbucket pipeline execution log attached as `.txt` | **Output:** 8-section diagnostic & optimization assessment  
> **Target / Tested With:** Any LLM · Cross-listed in [`../troubleshooting-debugging/readme.md`](../troubleshooting-debugging/readme.md)

## Debugging Bitbucket

<details>
<summary>🛠️ Comprehensive Bitbucket Pipeline Log Analysis Prompt</summary>

```text
Analyze the following Bitbucket pipeline execution log. Perform a thorough analysis of the Bitbucket pipeline execution log, covering various aspects such as execution status, errors, performance, and potential improvements.

Please provide a comprehensive assessment of the log, including:

1. Overall execution status (success, failure, or partial success)
2. Pipeline steps executed and their individual outcomes
3. Any errors or warnings encountered during execution
4. Performance metrics (if available), such as execution time for each step and overall pipeline
5. Resource usage information (if present in the logs)
6. Identification of any bottlenecks or areas for potential optimization
7. Suggestions for improving the pipeline based on the log analysis
8. Any unusual patterns or anomalies in the log that might require further investigation

Additionally, please highlight any critical issues that may require immediate attention and provide a brief summary of the key findings from the log analysis.

The log output is attached as a text file.
```

</details>

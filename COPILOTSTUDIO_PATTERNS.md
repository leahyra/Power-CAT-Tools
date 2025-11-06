## Power Platform Review Tool – Copilot Studio Agent Patterns

The following table lists key Copilot Studio Agent patterns used in the **Power Platform Review Tool**.  
These patterns are designed to evaluate and ensure best practices for **Copilot Studio Agents (Classic Orchestration-based)**.  
Each pattern helps identify potential improvements in topic design, trigger phrase quality, and overall agent performance.  

| **#** | **Pattern Name** | **Description** |
|:--:|:-----------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1 | **Trigger Phrase Count** | Ensures each topic contains at least 5 trigger phrases, helping bots respond to a wider variety of user queries. |
| 2 | **Single Word Phrases** | Identifies single-word trigger phrases and recommends using multi-word phrases for more accurate and meaningful responses. |
| 3 | **Long Phrases** | Flags trigger phrases exceeding 10 words in length, encouraging shorter and more concise queries for better bot performance. |
| 4 | **Condition Count** | Checks if topics contain too many condition action branches. |
| 5 | **Flow Count** | Checks the number of unique `flowIds` used in `InvokeFlowAction` and fails if more than 10 are found. |
| 6 | **SharePoint Auth Mode** | Checks if any SharePoint knowledge sources use **‘No Authentication’** as the authentication mode. |
| 7 | **Unused Topics** | Identifies topics without trigger phrases that are not referenced in any other topics. |
| 8 | **Synonyms Quality** | Validates synonyms in `ClosedListEntity` items to ensure no synonym exceeds 2 words. |
| 9 | **Duplicate Regex Entities** | Checks if multiple `RegexEntity` entities share the same regex pattern. |
| 10 | **End Of Conversation Usage** | Verifies at least one **End Of Conversation** topic exists (with `CancelOtherTopics` and a *Resolved* outcome) and that at least one topic references it. |

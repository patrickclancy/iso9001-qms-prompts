# Roles and Outputs

| Prompt | AI role | Main input | Main output | Who should review the output |
|---|---|---|---|---|
| 00 | Word document auditor | Word document | Audit packet | Document Control |
| 01 | Transformation analyst | Before audit + after audit | Pair comparison | Quality or editor |
| 02 | Rule-mining specialist | Pair comparison | Extracted rules | Quality or editor |
| 03 | Rule consolidator | Five extracted rule files | Master rulebook draft | Quality, Document Control, process owner |
| 04 | Prompt builder | Approved rulebook | Production reviewer prompt | Quality, prompt owner |
| 05 | QMS document reviewer | New document audit | Review findings | Process owner, Quality |
| 06 | QMS document editor | Review findings + audit | Rewritten content | Process owner, Quality |
| 07 | Word formatting reviewer | Revised document audit | Formatting report | Document Control |
| 08 | Final QA gate | Before audit + revised audit + findings | Release-readiness report | Quality, Document Control |

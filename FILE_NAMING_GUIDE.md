# File Naming Guide

Use consistent names so the user does not mix up before and after documents.

## Original Word files

```text
Pair01_Before.docx
Pair01_After.docx
Pair02_Before.docx
Pair02_After.docx
Pair03_Before.docx
Pair03_After.docx
Pair04_Before.docx
Pair04_After.docx
Pair05_Before.docx
Pair05_After.docx
```

## Prompt 00 outputs

```text
Pair01_Before_Audit.md
Pair01_After_Audit.md
Pair02_Before_Audit.md
Pair02_After_Audit.md
Pair03_Before_Audit.md
Pair03_After_Audit.md
Pair04_Before_Audit.md
Pair04_After_Audit.md
Pair05_Before_Audit.md
Pair05_After_Audit.md
```

## Prompt 01 outputs

```text
Pair01_Transformation_Analysis.md
Pair02_Transformation_Analysis.md
Pair03_Transformation_Analysis.md
Pair04_Transformation_Analysis.md
Pair05_Transformation_Analysis.md
```

## Prompt 02 outputs

```text
Pair01_Extracted_Rules.md
Pair02_Extracted_Rules.md
Pair03_Extracted_Rules.md
Pair04_Extracted_Rules.md
Pair05_Extracted_Rules.md
```

## Prompt 03 output

```text
Master_Consolidated_Rulebook_Draft.md
Master_Consolidated_Rulebook_Approved.md
```

## Prompt 04 output

```text
Production_Reviewer_Prompt.md
```

## New document production outputs

Use the document name instead of `New_Document` if possible.

```text
New_Before.docx
New_Before_Audit.md
New_Document_Review_Findings.md
New_Document_Rewritten_Content.md
New_After_Draft.docx
New_After_Draft_Audit.md
New_After_Draft_Formatting_Check.md
New_After_Final_QA_Report.md
```

## Simple rule

Never overwrite old outputs. Add a version number when needed.

Example:

```text
Master_Consolidated_Rulebook_Draft_v1.md
Master_Consolidated_Rulebook_Draft_v2.md
Master_Consolidated_Rulebook_Approved_v1.md
```

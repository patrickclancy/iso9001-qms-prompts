# Order of Operations

Follow this order exactly. Each step creates an output needed by a later step.

## Phase 1: Build the reviewer system from five before/after pairs

### Step 1 — Name the files

Use this naming pattern:

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

### Step 2 — Create audit packets for every document

Use:

```text
prompts/00_document_audit_packet/prompt.md
```

Run it once for every before and after document.

You should end with 10 audit packets:

```text
Pair01_Before_Audit.md
Pair01_After_Audit.md
...
Pair05_Before_Audit.md
Pair05_After_Audit.md
```

### Step 3 — Compare each before/after pair

Use:

```text
prompts/01_pairwise_transformation_analysis/prompt.md
```

Run it once per pair.

Inputs for Pair 01:

```text
Pair01_Before_Audit.md
Pair01_After_Audit.md
```

Output:

```text
Pair01_Transformation_Analysis.md
```

Repeat for all five pairs.

### Step 4 — Extract rules from each pair

Use:

```text
prompts/02_rule_extraction/prompt.md
```

Run it once for each transformation analysis.

Input:

```text
Pair01_Transformation_Analysis.md
```

Output:

```text
Pair01_Extracted_Rules.md
```

Repeat for all five pairs.

### Step 5 — Consolidate all rules

Use:

```text
prompts/03_cross_pair_rule_consolidation/prompt.md
```

Inputs:

```text
Pair01_Extracted_Rules.md
Pair02_Extracted_Rules.md
Pair03_Extracted_Rules.md
Pair04_Extracted_Rules.md
Pair05_Extracted_Rules.md
```

Output:

```text
Master_Consolidated_Rulebook_Draft.md
```

### Step 6 — Human approval of rules

A human reviewer should approve the rulebook before production use.

Recommended reviewers:

- Quality Manager
- Document Control owner
- Process owner
- Technical writer or editor

Output:

```text
Master_Consolidated_Rulebook_Approved.md
```

### Step 7 — Create production reviewer prompt

Use:

```text
prompts/04_reviewer_rulebook_generation/prompt.md
```

Inputs:

```text
Master_Consolidated_Rulebook_Approved.md
Company_Style_Requirements.md
Word_Formatting_Requirements.md
```

Output:

```text
Production_Reviewer_Prompt.md
```

## Phase 2: Review and rewrite new documents

### Step 8 — Audit the new document

Use Prompt 00 again.

Input:

```text
New_Before.docx
```

Output:

```text
New_Before_Audit.md
```

### Step 9 — Review the new document

Use:

```text
prompts/05_production_review/prompt.md
```

Inputs:

```text
New_Before_Audit.md
Master_Consolidated_Rulebook_Approved.md
Word_Formatting_Requirements.md
```

Output:

```text
New_Document_Review_Findings.md
```

### Step 10 — Rewrite the new document

Use:

```text
prompts/06_rewrite_before_to_after/prompt.md
```

Inputs:

```text
New_Before_Audit.md
Master_Consolidated_Rulebook_Approved.md
New_Document_Review_Findings.md
Word_Formatting_Requirements.md
```

Output:

```text
New_Document_Rewritten_Content.md
```

### Step 11 — Create the revised Word document

A person creates or updates the Word document using the rewritten content.

Apply the correct Word styles. Do not manually fake formatting by using only bold, font size, or spaces.

Output:

```text
New_After_Draft.docx
```

### Step 12 — Audit the revised Word document

Use Prompt 00 on the revised Word document.

Output:

```text
New_After_Draft_Audit.md
```

### Step 13 — Check Word formatting compliance

Use:

```text
prompts/07_word_formatting_compliance/prompt.md
```

Inputs:

```text
New_After_Draft_Audit.md
Word_Formatting_Requirements.md
Master_Consolidated_Rulebook_Approved.md
```

Output:

```text
New_After_Draft_Formatting_Check.md
```

### Step 14 — Run final QA gate

Use:

```text
prompts/08_final_qa_gate/prompt.md
```

Inputs:

```text
New_Before_Audit.md
New_After_Draft_Audit.md
Master_Consolidated_Rulebook_Approved.md
New_Document_Review_Findings.md
New_After_Draft_Formatting_Check.md
```

Output:

```text
New_After_Final_QA_Report.md
```

### Step 15 — Human release decision

If the final QA says the document is ready, send it to the normal approval process.

If the final QA says it needs revision, fix the issues and repeat Steps 12 through 14.

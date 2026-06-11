# Beginner Workflow Checklist

Print this checklist or copy it into your project notes.

## Setup

- [ ] Create a project folder.
- [ ] Add the five before documents.
- [ ] Add the five after documents.
- [ ] Rename documents using the Pair01, Pair02 naming pattern.
- [ ] Add the company style guide, if available.
- [ ] Add the Word template or formatting requirements, if available.
- [ ] Fill out `examples/style_requirements_template.md` if no formal style guide exists.

## Learning phase

### Prompt 00: Audit each document

- [ ] Run Prompt 00 on Pair01_Before.docx.
- [ ] Save output as Pair01_Before_Audit.md.
- [ ] Run Prompt 00 on Pair01_After.docx.
- [ ] Save output as Pair01_After_Audit.md.
- [ ] Repeat for Pair02 through Pair05.

Expected output count: 10 audit files.

### Prompt 01: Compare each pair

- [ ] Run Prompt 01 using Pair01_Before_Audit.md and Pair01_After_Audit.md.
- [ ] Save output as Pair01_Transformation_Analysis.md.
- [ ] Repeat for Pair02 through Pair05.

Expected output count: 5 transformation analysis files.

### Prompt 02: Extract pair rules

- [ ] Run Prompt 02 using Pair01_Transformation_Analysis.md.
- [ ] Save output as Pair01_Extracted_Rules.md.
- [ ] Repeat for Pair02 through Pair05.

Expected output count: 5 extracted rule files.

### Prompt 03: Create master rulebook

- [ ] Run Prompt 03 using all five extracted rule files.
- [ ] Save output as Master_Consolidated_Rulebook_Draft.md.

### Human approval

- [ ] Send the draft rulebook to Quality.
- [ ] Send the draft rulebook to Document Control.
- [ ] Send the draft rulebook to one process owner.
- [ ] Mark rules as Approved, Rejected, or Needs Change.
- [ ] Save the approved version as Master_Consolidated_Rulebook_Approved.md.

### Prompt 04: Create production reviewer prompt

- [ ] Run Prompt 04 using the approved rulebook.
- [ ] Save output as Production_Reviewer_Prompt.md.

## Production phase for a new document

- [ ] Run Prompt 00 on the new before document.
- [ ] Save output as New_Before_Audit.md.
- [ ] Run Prompt 05 to review the document.
- [ ] Save output as New_Document_Review_Findings.md.
- [ ] Run Prompt 06 to rewrite the document.
- [ ] Save output as New_Document_Rewritten_Content.md.
- [ ] Update the Word document using the rewritten content and style instructions.
- [ ] Save the revised Word document as New_After_Draft.docx.
- [ ] Run Prompt 00 on New_After_Draft.docx.
- [ ] Save output as New_After_Draft_Audit.md.
- [ ] Run Prompt 07 to check formatting.
- [ ] Save output as New_After_Draft_Formatting_Check.md.
- [ ] Run Prompt 08 for final QA.
- [ ] Save output as New_After_Final_QA_Report.md.
- [ ] Send to normal human approval process.

## Stop signs

Stop and ask for human review if the AI flags:

- [ ] A possible change in meaning.
- [ ] A missing responsibility.
- [ ] A missing approval.
- [ ] A missing record.
- [ ] A change to shall, must, should, may, approve, verify, retain, or maintain.
- [ ] A conflict between the examples and the company style guide.
- [ ] A formatting requirement that is unclear.


## Helper prompt checklist for small edits

Use this checklist when you only need to polish one section, paragraph, step, table row, or process map.

- [ ] Open `helper_prompts/HELPER_SELECTION_GUIDE.md`.
- [ ] Choose the helper that matches the task.
- [ ] Copy the helper's `prompt.md` into your AI tool.
- [ ] Paste only the small text section that needs help.
- [ ] Fill in the common input block.
- [ ] Review the proposed revised text.
- [ ] Run `helper_prompts/15_meaning_guard_compare_helper/prompt.md` if the change affects requirements, responsibilities, approvals, records, scope, or sequence.
- [ ] Save the original text and approved revised text in your project notes.
- [ ] Paste the approved text into Word using the required Word style.
- [ ] Ask Quality or the process owner to approve any flagged meaning-impact item.

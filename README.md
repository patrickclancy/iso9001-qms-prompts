# ISO 9001:2015 QMS Document Reviewer Prompt Development Archive

This archive contains a complete, beginner-friendly prompt kit for building a reviewer system that can evaluate and improve ISO 9001:2015 policy and procedure Word documents.

The goal is to learn from approximately five **before/after** document pairs and turn the observed improvements into a reusable reviewer and rewrite process.

## What this kit helps you do

Use this kit to:

1. Compare old Word documents to improved Word documents.
2. Discover the writing, structure, tone, readability, and formatting rules used in the improved documents.
3. Build a reusable reviewer rulebook.
4. Review new documents using the learned rules.
5. Rewrite new documents into the approved after-document style.
6. Check final documents before release.

## Who this is for

This kit is written for a non-technical user. The user only needs to know how to:

- Open a Markdown file.
- Copy and paste a prompt into an AI tool.
- Upload Word documents when requested.
- Save the AI output into a file or document.
- Follow the numbered steps in order.

## Important safety rule

Do not let the AI invent ISO requirements, process steps, responsibilities, approvals, or records. The prompts in this kit repeatedly instruct the AI to preserve the document's meaning and flag gaps for human review.

## Folder overview

```text
iso9001_qms_prompt_development_archive/
├── README.md
├── START_HERE.md
├── ORDER_OF_OPERATIONS.md
├── BEGINNER_WORKFLOW_CHECKLIST.md
├── FILE_NAMING_GUIDE.md
├── GLOSSARY.md
├── ARCHIVE_MANIFEST.md
├── examples/
│   ├── document_pair_log_template.md
│   ├── file_tracker_template.md
│   ├── findings_table_template.md
│   ├── rulebook_template.md
│   └── style_requirements_template.md
├── prompts/
│   ├── 00_document_audit_packet/
│   │   ├── README.md
│   │   └── prompt.md
│   ├── 01_pairwise_transformation_analysis/
│   │   ├── README.md
│   │   └── prompt.md
│   ├── 02_rule_extraction/
│   │   ├── README.md
│   │   └── prompt.md
│   ├── 03_cross_pair_rule_consolidation/
│   │   ├── README.md
│   │   └── prompt.md
│   ├── 04_reviewer_rulebook_generation/
│   │   ├── README.md
│   │   └── prompt.md
│   ├── 05_production_review/
│   │   ├── README.md
│   │   └── prompt.md
│   ├── 06_rewrite_before_to_after/
│   │   ├── README.md
│   │   └── prompt.md
│   ├── 07_word_formatting_compliance/
│   │   ├── README.md
│   │   └── prompt.md
│   └── 08_final_qa_gate/
│       ├── README.md
│       └── prompt.md
└── quick_reference/
    ├── copy_paste_order.md
    ├── decision_tree.md
    └── roles_and_outputs.md
```

## Main process at a glance

There are two phases.

### Phase 1: Learn the rules from existing before/after documents

Use Prompts 00 through 04.

```text
Prompt 00: Create an audit packet for each Word document.
Prompt 01: Compare each before/after pair.
Prompt 02: Extract reusable rules from each pair.
Prompt 03: Combine all pair rules into one master rulebook.
Prompt 04: Turn the master rulebook into a production reviewer prompt.
```

### Phase 2: Use the approved rules on new documents

Use Prompts 05 through 08.

```text
Prompt 05: Review a new before document.
Prompt 06: Rewrite the document into after style.
Prompt 07: Check Word formatting compliance.
Prompt 08: Perform final QA gate review.
```



## Targeted helper prompts

This archive also includes a `helper_prompts/` folder for small, targeted edits.

Use these helpers when you do not want a large rewrite and only need to polish one section, paragraph, process step, table row, or activity map.

Common examples:

- Purpose section cleanup.
- Scope section cleanup.
- Key Requirements polishing.
- One procedure step cleanup.
- Long paragraph converted to steps.
- Process activity map draft.
- Meaning-check comparison between original and revised wording.

Start here:

```text
helper_prompts/HELPER_PROMPTS_START_HERE.md
```

For a quick selection table, open:

```text
helper_prompts/HELPER_SELECTION_GUIDE.md
```

## Recommended naming convention

Use simple names like this:

```text
Pair01_Before.docx
Pair01_After.docx
Pair02_Before.docx
Pair02_After.docx
...
Pair05_Before.docx
Pair05_After.docx
```

Save AI outputs with matching names:

```text
Pair01_Before_Audit.md
Pair01_After_Audit.md
Pair01_Transformation_Analysis.md
Pair01_Extracted_Rules.md
```

See `FILE_NAMING_GUIDE.md` for the complete naming system.

## Required human approvals

Before using the final reviewer prompt in production, a human should approve:

- The consolidated rulebook.
- The company Word formatting requirements.
- Any rules that change wording such as shall, must, should, may, approve, verify, retain, maintain, or responsible for.
- Any rules affecting document control, approval, records, or responsibilities.

## Best practice

Keep one clean folder for each document pair. Do not mix outputs from different pairs. The AI will perform better when each step has clear input files.

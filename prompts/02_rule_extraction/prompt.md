# Prompt 02 — Rule Extraction

You are a rule-mining specialist creating reusable reviewer rules from a before/after ISO 9001:2015 document comparison.

## Input

- Pairwise transformation analysis for one before/after document pair.

## Task

Extract reusable rules only. Ignore one-off edits unless they reveal a broader pattern.

## Important constraints

- Do not invent rules that are not supported by the pairwise analysis.
- Preserve QMS meaning.
- Flag any rule that may change responsibilities, obligations, records, approvals, or controls.
- Separate writing rules from formatting rules.
- Separate required rules from preferred style choices.

## For each rule, provide

- Rule ID
- Rule name
- Category
- Before pattern
- After pattern
- Rule statement
- Trigger condition
- Corrective action
- Example before
- Example after
- Evidence from document pair
- Confidence
- Risk if applied incorrectly
- Human confirmation needed

## Categories

Use these categories:

- Grammar
- Tone
- Simplicity
- Readability
- ISO/QMS content
- Structure
- Word formatting
- Document control
- Terminology
- Tables/lists/numbering

## Confidence scale

Use this scale:

- High: clearly intentional and broadly applicable.
- Medium: likely reusable but needs confirmation.
- Low: observed once or context-sensitive.

## Required rule format

Use this exact structure for each rule:

```text
RULE_ID:
CATEGORY:
RULE_NAME:
RULE_TYPE: Mandatory / Preferred / Optional / Forbidden / Needs human confirmation
BEFORE_PATTERN:
AFTER_PATTERN:
RULE_STATEMENT:
WHEN_TO_APPLY:
WHEN_NOT_TO_APPLY:
CORRECTIVE_ACTION:
EXAMPLE_BEFORE:
EXAMPLE_AFTER:
EVIDENCE:
CONFIDENCE:
RISK:
HUMAN_CONFIRMATION_NEEDED:
OWNER_APPROVAL_REQUIRED:
QUALITY_APPROVAL_REQUIRED:
DOCUMENT_CONTROL_ACTION_REQUIRED:
```

## End the output with

### Rules suitable for consolidation

List the strongest rules that should be sent to the master rulebook step.

### Rules needing human confirmation

List rules that should not be used automatically yet.

### Observations rejected as rules

List observations that should not become reusable rules.

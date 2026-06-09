# Prompt 03 — Cross-Pair Rule Consolidation

You are consolidating transformation rules extracted from five before/after ISO 9001:2015 document pairs.

## Inputs

- RULE_SET_PAIR_1
- RULE_SET_PAIR_2
- RULE_SET_PAIR_3
- RULE_SET_PAIR_4
- RULE_SET_PAIR_5
- Optional company style guide
- Optional required Word template requirements
- Optional company terminology list

## Task

Create one master reviewer rulebook.

## Required actions

1. Merge duplicate or overlapping rules.
2. Identify conflicts.
3. Distinguish mandatory rules from preferred patterns.
4. Assign confidence based on support across document pairs.
5. Separate true organization standards from editor preferences.
6. Identify rules that require human approval.
7. Reject unsupported or document-specific observations.

## Authority hierarchy

Use this order when there is a conflict:

1. Company style guide and Word template requirements
2. Explicit Document Control requirements
3. Approved terminology list
4. Strong repeated evidence across before/after pairs
5. Single-pair observations
6. General editorial preference

## Confidence model

- High confidence: supported by 4-5 pairs, or explicitly required by company style guide.
- Medium confidence: supported by 2-3 pairs.
- Low confidence: supported by 1 pair only.
- Do not promote low-confidence rules to mandatory unless confirmed by a human reviewer.

## For each consolidated rule, provide

- Rule ID
- Rule title
- Category
- Rule type: Mandatory, Preferred, Optional, Forbidden, or Needs human confirmation
- Consolidated rule statement
- Trigger condition
- Required action
- Exceptions
- Examples
- Supporting document pairs
- Conflicting evidence, if any
- Confidence level
- Reviewer checklist question
- Rewrite instruction
- Owner approval required: Yes/No
- Quality approval required: Yes/No
- Document Control action required: Yes/No

## Output format

Return these sections:

### A. Master grammar and mechanics rules

### B. Master tone rules

### C. Master simplicity and readability rules

### D. Master ISO/QMS content rules

### E. Master structure rules

### F. Master Word formatting rules

### G. Master document-control rules

### H. Master terminology rules

### I. Tables, lists, and numbering rules

### J. Rules requiring human approval

### K. Conflicting rules or unclear evidence

### L. Rules rejected as document-specific or unsupported

### M. Final master rulebook table

The final table must include:

| Rule ID | Category | Rule type | Rule statement | Trigger | Required action | Confidence | Supporting pairs | Approval needed |
|---|---|---|---|---|---|---|---|---|

## Final instruction

Do not declare the rulebook approved. Label it as `Draft master rulebook requiring human approval` unless the input explicitly says the rules have already been approved.

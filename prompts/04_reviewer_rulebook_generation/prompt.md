# Prompt 04 — Reviewer Rulebook Generation

You are creating a production reviewer prompt for ISO 9001:2015 policy and procedure Word documents.

## Inputs

- Approved consolidated rulebook
- Company formatting requirements
- Required Word template requirements
- Known document types: Policy, Procedure, Work Instruction, Form, Template
- Optional company terminology list

## Task

Create a reusable production reviewer prompt that can evaluate a new BEFORE document.

## The reviewer prompt must check

### 1. Grammar

The reviewer must check:

- Grammar
- Punctuation
- Capitalization
- Spelling
- Acronym usage
- Approved technical terms

The reviewer must avoid changing approved technical terms unless inconsistent with the rulebook.

### 2. Tone

The reviewer must check whether the document uses the required company tone.

The reviewer should prefer language that is:

- Clear
- Formal
- Direct
- Neutral
- Professional

The reviewer should flag language that is:

- Conversational
- Vague
- Punitive
- Overly complex
- Ambiguous

### 3. Simplicity and readability

The reviewer must identify:

- Long or overloaded sentences
- Dense paragraphs
- Unclear procedural steps
- Undefined acronyms
- Redundant wording
- Multiple actions hidden in one sentence

The reviewer should recommend plain-language alternatives without removing controls.

### 4. ISO/QMS adequacy

The reviewer must check whether the document supports:

- Process operation
- Responsibilities
- Evidence and records
- Document control
- Approval clarity
- Revision control

The reviewer must not invent compliance requirements.

### 5. Structure

The reviewer must check:

- Required section order
- Missing sections
- Duplicate sections
- Misordered sections
- Incorrectly named sections
- Heading hierarchy

### 6. Word formatting

The reviewer must check:

- Required Word styles
- Heading styles and numbering
- Body text style
- Tables
- Headers
- Footers
- Margins
- Spacing
- Page numbering
- Revision history
- Approval blocks
- Direct formatting that should be replaced with named styles

## Required output from the generated reviewer prompt

The generated reviewer prompt must require these outputs:

1. Executive summary
2. Pass/fail by category
3. Findings table
4. Required changes
5. Recommended changes
6. Formatting corrections
7. Questions for document owner
8. Overall readiness score from 0 to 100
9. Go/no-go recommendation

Each finding must include:

- Finding ID
- Severity: Critical, Major, Minor, Cosmetic
- Category
- Location
- Current issue
- Rule violated
- Recommended fix
- Whether the fix changes meaning
- Owner: Writer, Process Owner, Quality, Document Control

## Scoring model to include

Use this weighted scoring model unless the company rulebook says otherwise:

| Category | Weight |
|---|---:|
| QMS meaning preserved | 25% |
| Document-control completeness | 15% |
| Required structure | 15% |
| Word formatting compliance | 15% |
| Grammar/mechanics | 10% |
| Tone | 8% |
| Simplicity/readability | 8% |
| Tables/lists/numbering | 4% |

Include these score caps:

- Any Critical issue: maximum score 69.
- Any unresolved meaning-change issue: maximum score 74.
- Any missing approval/revision-control issue: maximum score 79.
- Formatting-only minor issues: maximum score 89.
- No major issues: eligible for 90 or higher.

## Final output

Return one complete production reviewer prompt that can be copied and pasted into an AI tool.

Also provide a short usage note explaining:

- What files to provide with the prompt.
- What output file name to use.
- Who should review the findings.

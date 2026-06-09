# Master Rulebook Template

Use this structure for the approved reviewer rulebook.

## Rule format

```text
RULE_ID:
CATEGORY:
RULE_TITLE:
RULE_TYPE: Mandatory / Preferred / Optional / Forbidden / Needs human confirmation
RULE_STATEMENT:
TRIGGER_CONDITION:
REQUIRED_ACTION:
EXCEPTIONS:
EXAMPLE_BEFORE:
EXAMPLE_AFTER:
SUPPORTING_DOCUMENT_PAIRS:
CONFLICTING_EVIDENCE:
CONFIDENCE: High / Medium / Low
REVIEWER_CHECKLIST_QUESTION:
REWRITE_INSTRUCTION:
OWNER_APPROVAL_REQUIRED: Yes / No
QUALITY_APPROVAL_REQUIRED: Yes / No
DOCUMENT_CONTROL_ACTION_REQUIRED: Yes / No
```

## Example rule

```text
RULE_ID: FORMAT-001
CATEGORY: Word Formatting
RULE_TITLE: Use approved heading styles
RULE_TYPE: Mandatory
RULE_STATEMENT: All headings must use approved Word heading styles rather than manual bold formatting.
TRIGGER_CONDITION: Text appears to be a heading but uses Normal, Body Text, or direct formatting.
REQUIRED_ACTION: Apply the correct approved Word heading style.
EXCEPTIONS: None.
EXAMPLE_BEFORE: A bold paragraph using Normal style.
EXAMPLE_AFTER: The same heading using Heading 1 or Heading 2 style.
SUPPORTING_DOCUMENT_PAIRS: Pair01, Pair02, Pair04
CONFLICTING_EVIDENCE: None.
CONFIDENCE: High
REVIEWER_CHECKLIST_QUESTION: Are all headings created using approved Word styles?
REWRITE_INSTRUCTION: Map each heading to the appropriate approved Word style.
OWNER_APPROVAL_REQUIRED: No
QUALITY_APPROVAL_REQUIRED: No
DOCUMENT_CONTROL_ACTION_REQUIRED: Yes
```

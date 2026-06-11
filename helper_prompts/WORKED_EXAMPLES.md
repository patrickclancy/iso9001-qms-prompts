# Worked Examples for Helper Prompts

These examples show how a non-technical user can use the helper prompts.

The examples are generic. Replace the sample text with your actual document text.

---

## Example 1 — Purpose section cleanup

### Helper to use

```text
helper_prompts/01_purpose_section_helper/prompt.md
```

### Input to paste below the prompt

```text
Document type:
Procedure

Document title:
Supplier Evaluation Procedure

Section being edited:
Purpose

Current text to improve:
This procedure is to explain how we look at suppliers and make sure they are okay to use and keep using.

Approved rulebook or style rules to apply:
Use formal QMS tone. Keep wording clear and concise. Do not add requirements.

Company terminology that must be preserved:
Supplier, Approved Supplier List, Quality Manager

Words or meaning that must not change:
The document controls supplier evaluation and continued use.

Specific concern:
Tone is too informal.
```

### Type of output to expect

```text
The purpose of this procedure is to define the process for evaluating, approving, and monitoring suppliers to ensure they remain suitable for use.
```

Before accepting it, check whether "monitoring" is already part of the procedure. If not, ask the process owner.

---

## Example 2 — Scope section cleanup

### Helper to use

```text
helper_prompts/02_scope_section_helper/prompt.md
```

### Input to paste below the prompt

```text
Document type:
Procedure

Document title:
Document Control Procedure

Section being edited:
Scope

Current text to improve:
This applies to documents and records used by the company.

Approved rulebook or style rules to apply:
Use clear boundaries. Do not invent exclusions.

Company terminology that must be preserved:
QMS documents, records, Document Control

Words or meaning that must not change:
Applies to company documents and records.

Specific concern:
Scope is too vague.
```

### Type of output to expect

The helper should make the wording clearer and list questions such as:

```text
Does this apply to all locations?
Does this apply to external documents?
Does this apply to electronic records?
```

Do not let the helper answer those questions unless you provide the facts.

---

## Example 3 — Convert a dense paragraph into steps

### Helper to use

```text
helper_prompts/07_paragraph_to_steps_helper/prompt.md
```

### Input to paste below the prompt

```text
Document type:
Procedure

Document title:
Corrective Action Procedure

Section being edited:
Procedure steps

Current text to improve:
The Quality Manager reviews the issue, assigns an owner, determines whether containment is needed, and verifies that the corrective action was completed before closing the corrective action record.

Approved rulebook or style rules to apply:
Use one main action per step. Preserve process sequence and responsibilities.

Company terminology that must be preserved:
Quality Manager, corrective action record

Words or meaning that must not change:
Quality Manager reviews, assigns owner, determines containment, verifies completion, closes record.

Specific concern:
Sentence contains too many actions.
```

### Type of output to expect

```text
1. The Quality Manager reviews the issue.
2. The Quality Manager assigns an owner.
3. The Quality Manager determines whether containment is required.
4. The assigned owner completes the corrective action.
5. The Quality Manager verifies completion before closing the corrective action record.
```

Then run the meaning guard helper because the output introduced "assigned owner completes the corrective action." That may be correct, but it should be confirmed if the original sentence did not clearly say who completes the action.

---

## Example 4 — Create a process activity map

### Helper to use

```text
helper_prompts/08_process_activity_map_helper/prompt.md
```

### Input to paste below the prompt

```text
Document type:
Procedure

Document title:
Nonconforming Output Procedure

Section being edited:
Process activity map

Current text to improve:
1. Employee identifies nonconforming output.
2. Employee segregates or identifies the output to prevent unintended use.
3. Quality reviews the nonconformance.
4. Quality determines disposition.
5. Authorized personnel approve the disposition.
6. The disposition is completed and recorded.

Approved rulebook or style rules to apply:
Use a Word-friendly activity map. Do not invent steps.

Company terminology that must be preserved:
Employee, Quality, authorized personnel, nonconforming output

Words or meaning that must not change:
Identification, segregation, Quality review, disposition, approval, record.

Specific concern:
Need a simple diagram for the procedure.
```

### Type of output to expect

The helper should return a simple box-and-arrow map and a swimlane table. After that, use:

```text
helper_prompts/16_activity_map_validation_helper/prompt.md
```

---

## Example 5 — Meaning guard check

### Helper to use

```text
helper_prompts/15_meaning_guard_compare_helper/prompt.md
```

### Input to paste below the prompt

```text
ORIGINAL TEXT:
The Quality Manager shall approve all supplier re-evaluations.

REVISED TEXT:
The Quality Manager may approve supplier re-evaluations.

Approved rulebook or style rules to apply:
Mandatory requirements use shall.

Terms or obligations that must not change:
Quality Manager, approve, supplier re-evaluations, shall.
```

### Type of output to expect

The helper should flag this as unsafe because `shall approve all` changed to `may approve`.

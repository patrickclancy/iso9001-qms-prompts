# Helper Selection Guide

Use this guide to choose the right helper prompt.

| What you want to do | Use this helper |
|---|---|
| I have a paragraph and I just want it cleaner. | `00_general_section_polisher` |
| I need a clearer Purpose section. | `01_purpose_section_helper` |
| I need to clarify where the document applies. | `02_scope_section_helper` |
| I need to polish shall/must/key requirement bullets. | `03_key_requirements_helper` |
| I need to polish a policy statement. | `04_policy_statement_helper` |
| I need to clarify who does what. | `05_responsibilities_helper` |
| I need to clean up one procedure step. | `06_process_step_polisher` |
| I have a long paragraph that should become numbered steps. | `07_paragraph_to_steps_helper` |
| I need a process activity map or swimlane table. | `08_process_activity_map_helper` |
| I need to clean up inputs, outputs, records, or evidence. | `09_inputs_outputs_records_helper` |
| I need to clean up definitions or acronyms. | `10_definitions_acronyms_helper` |
| I need to clean up references or related documents. | `11_references_related_documents_helper` |
| I need to polish a row in a table. | `12_table_content_polisher` |
| I need to rewrite a note, caution, or warning. | `13_note_caution_warning_helper` |
| I only need one sentence polished. | `14_micro_sentence_polisher` |
| I need to check whether a rewrite changed the meaning. | `15_meaning_guard_compare_helper` |
| I need to check if the activity map matches the steps. | `16_activity_map_validation_helper` |

## Recommended order for a procedure section rewrite

Use this order when building or improving a procedure section by section:

```text
1. Purpose helper
2. Scope helper
3. Responsibilities helper
4. Key Requirements helper
5. Process Step Polisher or Paragraph-to-Steps helper
6. Inputs/Outputs/Records helper
7. Process Activity Map helper
8. Activity Map Validation helper
9. Meaning Guard helper for any sensitive changes
```

## Recommended order for a policy section rewrite

```text
1. Purpose helper
2. Scope helper
3. Policy Statement helper
4. Key Requirements helper
5. Responsibilities helper
6. References/Related Documents helper
7. Meaning Guard helper for any sensitive changes
```

## Use the meaning guard more often than you think

A sentence can look better but become weaker.

Example:

```text
Original: The Quality Manager shall approve supplier re-evaluations.
Risky rewrite: The Quality Manager may approve supplier re-evaluations.
```

That is not just a wording improvement. It changes a mandatory approval into an optional one.

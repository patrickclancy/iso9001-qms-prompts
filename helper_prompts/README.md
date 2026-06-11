# Helper Prompts for Targeted ISO 9001:2015 QMS Content Polishing

This folder contains small, focused prompts for cleaning up individual sections of a policy, procedure, work instruction, or controlled QMS document.

These helpers are different from the main reviewer/rewrite prompts. They are not designed to rewrite a full document. They are designed to polish one section, paragraph, table row, step, or process-flow fragment at a time.

## Use these helpers when you need to improve a small part of a document

Examples:

- Clean up a Purpose section.
- Tighten a Scope statement.
- Make Key Requirements clearer.
- Polish one procedure step.
- Convert a long paragraph into numbered process steps.
- Create a Word-friendly process activity map.
- Check whether a polished paragraph accidentally changed the meaning.

## Basic use

1. Open `HELPER_PROMPTS_START_HERE.md`.
2. Use `HELPER_SELECTION_GUIDE.md` to choose the right helper.
3. Open the helper folder.
4. Open `prompt.md`.
5. Copy the prompt into your AI tool.
6. Paste the requested text and context below the prompt.
7. Review the output before putting it into the Word document.
8. If the edit might change meaning, run `15_meaning_guard_compare_helper` before accepting it.

## Important safety rule

These prompts may improve wording, but they must not invent requirements, remove controls, change responsibilities, alter approval authority, change records, or weaken required actions.

If a helper changes words such as `shall`, `must`, `should`, `may`, `approve`, `verify`, `retain`, `maintain`, `responsible`, `record`, or `evidence`, send the before and after text through the meaning guard helper.

## Helper folders

| Folder | Use it for |
|---|---|
| `00_general_section_polisher` | Any short section or paragraph when you are not sure which helper to use. |
| `01_purpose_section_helper` | Purpose sections. |
| `02_scope_section_helper` | Scope sections, boundaries, inclusions, and exclusions. |
| `03_key_requirements_helper` | Key requirements, shall/must statements, and compliance bullets. |
| `04_policy_statement_helper` | Policy statements and management commitments. |
| `05_responsibilities_helper` | Responsibilities by role, department, or process owner. |
| `06_process_step_polisher` | One procedure step or short set of steps. |
| `07_paragraph_to_steps_helper` | Convert a dense paragraph into clear numbered steps. |
| `08_process_activity_map_helper` | Create a simple process activity map or swimlane table. |
| `09_inputs_outputs_records_helper` | Inputs, outputs, records, evidence, and retained information. |
| `10_definitions_acronyms_helper` | Definitions and acronym cleanup. |
| `11_references_related_documents_helper` | References and related documents sections. |
| `12_table_content_polisher` | Table rows, responsibility tables, records tables, and requirement tables. |
| `13_note_caution_warning_helper` | Notes, cautions, warnings, and reminders. |
| `14_micro_sentence_polisher` | One sentence at a time. |
| `15_meaning_guard_compare_helper` | Compare before/after text to detect unintended meaning changes. |
| `16_activity_map_validation_helper` | Check that a process map matches the written procedure steps. |

## Recommended review habit

For simple grammar-only edits, one helper may be enough.

For anything involving a requirement, responsibility, approval, record, or process sequence, use this pattern:

```text
1. Use the targeted helper.
2. Review the proposed text.
3. Run the meaning guard helper.
4. Ask the process owner or Quality reviewer to approve any meaning-impact item.
```


## Additional helper guides

| File | Use it for |
|---|---|
| `HELPER_ORDER_OF_OPERATIONS.md` | Step-by-step helper workflow for section cleanup, drafting, process steps, activity maps, and meaning checks. |
| `WORKED_EXAMPLES.md` | Simple examples showing exactly what to paste into a helper prompt. |
| `QUALITY_CHECKLIST_FOR_HELPER_OUTPUTS.md` | Checklist to use before pasting helper output into a controlled document. |

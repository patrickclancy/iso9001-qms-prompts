# Helper Prompt Order of Operations

Use this guide when you are polishing document content section by section.

The helper prompts are designed for targeted edits. Do not paste a full document into a helper prompt unless the prompt specifically asks for a short reference excerpt.

## Workflow A — Clean up one existing section

Use this when the Word document already has a section, but the wording needs improvement.

```text
Step 1: Choose one short section or paragraph.
Step 2: Open HELPER_SELECTION_GUIDE.md.
Step 3: Choose the matching helper.
Step 4: Copy the helper's prompt.md into your AI tool.
Step 5: Fill in the input block.
Step 6: Review the revised text.
Step 7: If meaning could have changed, run 15_meaning_guard_compare_helper.
Step 8: Save the approved revised text in your project notes.
Step 9: Paste the approved text into Word using the correct Word style.
```

## Workflow B — Draft a missing small section

Use this when a required section is missing, but you have enough source information to draft it.

```text
Step 1: Confirm the section is required by your approved rulebook or template.
Step 2: Gather source facts from the process owner or existing procedure text.
Step 3: Choose the matching helper.
Step 4: Paste only the source facts, not assumptions.
Step 5: Ask the helper to draft a short section and list questions.
Step 6: Send questions to the process owner or Quality reviewer.
Step 7: Do not release the section until answers are confirmed.
```

Important: If the source facts are missing, the helper should ask questions. It should not make up the missing information.

## Workflow C — Polish procedure steps

Use this when a procedure section is too wordy or hard to follow.

```text
Step 1: Select one paragraph or small group of steps.
Step 2: Use 07_paragraph_to_steps_helper if the paragraph contains several actions.
Step 3: Use 06_process_step_polisher for individual step cleanup.
Step 4: Run 15_meaning_guard_compare_helper on any step that affects responsibilities, approvals, records, or timing.
Step 5: Ask the process owner to approve any flagged change.
```

## Workflow D — Create a process activity map

Use this when you need a simple diagram or activity map for a procedure.

```text
Step 1: Finalize the written procedure steps first.
Step 2: Paste the steps into 08_process_activity_map_helper.
Step 3: Ask for a Word-friendly box-and-arrow map and a swimlane table.
Step 4: Review the map for missing steps, extra steps, or wrong sequence.
Step 5: Paste the written steps and draft map into 16_activity_map_validation_helper.
Step 6: Correct mismatches.
Step 7: Get process owner approval before release.
```

## Workflow E — Check meaning before accepting polished text

Use this when the AI revised wording that could affect QMS control.

```text
Step 1: Copy the original text.
Step 2: Copy the revised text.
Step 3: Open 15_meaning_guard_compare_helper/prompt.md.
Step 4: Paste both texts into the input block.
Step 5: Follow the decision:
        - Safe to use
        - Probably safe, minor review suggested
        - Needs process owner review
        - Needs Quality review
        - Do not use as written
```

## Simple rule for non-technical users

When the edit is only grammar, you can usually use the helper output after review.

When the edit affects what people must do, who approves, what record is kept, or where the procedure applies, use the meaning guard and get human approval.

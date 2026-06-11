# Helper Prompts Start Here

Use this file when you only need to improve a small part of a document.

Do not use these helpers for a full document rewrite. For a full document rewrite, use the main prompt:

```text
prompts/06_rewrite_before_to_after/prompt.md
```

## The simple process

### Step 1 — Pick the small piece you want to improve

Choose only one of these at a time:

- One Purpose section.
- One Scope section.
- One Key Requirements section.
- One paragraph.
- One procedure step.
- One table row.
- One small process-flow description.

Avoid pasting the whole document unless the helper specifically asks for a short reference excerpt.

### Step 2 — Choose the helper

Open `HELPER_SELECTION_GUIDE.md`.

Use the table to choose the right helper folder.

### Step 3 — Copy the prompt

Open the helper folder and copy the text in `prompt.md`.

Paste it into your AI tool.

### Step 4 — Add the input block

At the bottom of the prompt, fill in this information:

```text
Document type:
Document title:
Section being edited:
Current text to improve:
Approved rulebook or style rules to apply:
Company terminology that must be preserved:
Words or meaning that must not change:
Specific concern:
```

Do not worry if you do not have every item. Fill in what you know.

### Step 5 — Review the output

Look for these items:

- Did the wording become clearer?
- Did the meaning stay the same?
- Did a required action accidentally become optional?
- Did a role, approval, record, or responsibility change?
- Did the AI add something that was not in the original?

### Step 6 — Use the meaning guard when needed

Use `15_meaning_guard_compare_helper` when the edited text touches any of these:

- Shall, must, should, may.
- Approve, verify, review, inspect, retain, maintain.
- Responsible for.
- Records or evidence.
- Process sequence.
- Scope limits.
- Customer, regulatory, or statutory requirements.

### Step 7 — Paste only approved text into Word

Do not paste AI output directly into a controlled document unless the change is reviewed.

For QMS documents, the safest habit is:

```text
AI proposes. Human approves. Document Control formats and releases.
```

## Best first helper

If you are not sure which helper to use, start with:

```text
helper_prompts/00_general_section_polisher/prompt.md
```

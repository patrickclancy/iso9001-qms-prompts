# Prompt 00 — Document Audit Packet README

## Purpose

Use this prompt to turn a Word document into a structured audit packet. The audit packet is the input for later comparison, review, and formatting checks.

## When to use this prompt

Use this prompt on every before document, every after document, and every revised draft document.

## What to have ready

- One Word document
- Optional company style guide
- Optional Word formatting requirements

## Simple step-by-step instructions

1. Open `prompt.md` in this folder.
2. Copy the entire prompt.
3. Paste it into your AI tool.
4. Attach or paste the required input files.
5. Tell the AI which pair or document you are working on.
6. Review the AI response for warnings such as `human confirmation needed`.
7. Save the response using the file name listed below.

## Save the output as

```text
Pair##_Before_Audit.md or Pair##_After_Audit.md
```

## Expected output

A Markdown audit packet describing the document structure, text, formatting, tables, headers, footers, and document-control elements.

## What to do next

For before/after learning, run Prompt 01 after you have both audit packets for a pair. For production review, run Prompt 05 after auditing the new before document.

## Common mistakes to avoid

- Do not mix files from different before/after pairs.
- Do not skip saving the output.
- Do not treat low-confidence or human-confirmation items as approved rules.
- Do not allow the AI to invent missing responsibilities, records, approvals, or ISO requirements.
- Do not overwrite previous output files.

## Beginner tip

After the AI responds, copy the full response into a Markdown file. Use the file name recommended above. Keep it in the same project folder as the related document pair.

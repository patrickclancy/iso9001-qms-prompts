# Start Here

Use this page first. It explains the whole process in simple terms.

## What you need before starting

Collect the following files:

1. Five original documents. These are the **before** documents.
2. Five improved documents. These are the matching **after** documents.
3. Any company style guide, if available.
4. Any Word template or formatting requirements, if available.
5. Any company terminology list, if available.

## What is a before/after pair?

A before/after pair is one document before improvement and the matching document after improvement.

Example:

```text
Pair01_Before.docx = old supplier approval procedure
Pair01_After.docx  = improved supplier approval procedure
```

The AI compares each pair to learn what changed.

## The most important rule

Always keep each before document matched with the correct after document.

Do not compare the wrong documents.

## Simple process

### Learning phase

Use this phase once to build the rulebook.

```text
1. Run Prompt 00 on each Word document.
2. Run Prompt 01 on each before/after pair.
3. Run Prompt 02 on each pair analysis.
4. Run Prompt 03 on all extracted rules.
5. Ask a human reviewer to approve the consolidated rules.
6. Run Prompt 04 to create the production reviewer prompt.
```

### Production phase

Use this phase every time you review a new document.

```text
1. Run Prompt 00 on the new Word document.
2. Run Prompt 05 to review it.
3. Run Prompt 06 to rewrite it.
4. Run Prompt 00 again on the revised document.
5. Run Prompt 07 to check formatting.
6. Run Prompt 08 for final QA.
```

## What to copy and paste

Each prompt folder has two files:

```text
README.md = instructions for using that prompt
prompt.md = the actual prompt to copy and paste
```

Open the README first. Then copy the prompt.

## What to save

After each AI response, save the output. Use the suggested file names in the README for each prompt.

Example:

```text
Pair01_Before_Audit.md
Pair01_After_Audit.md
Pair01_Transformation_Analysis.md
Pair01_Extracted_Rules.md
```

## What to do if the AI says it cannot see Word formatting

Some AI tools can read Word formatting. Some cannot.

If the tool cannot inspect formatting directly, still run the prompt and ask it to analyze whatever it can see. Then have someone manually confirm Word-specific items such as:

- Styles
- Headings
- Fonts
- Margins
- Headers and footers
- Page numbers
- Table formatting
- Revision history formatting

## What to do when unsure

If the AI output says “human confirmation needed,” do not ignore it. Ask the document owner, Quality, or Document Control to confirm.

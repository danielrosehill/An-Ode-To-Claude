# Version Control System for Iterative Writing

This document describes a lightweight versioning system for prose and creative writing that tracks authorship across human and AI contributions.

## Purpose

When writing iteratively — especially with AI assistance — it's useful to maintain a clear record of who made what changes and why. This system provides that transparency.

## Structure

```
project-root/
├── iterations/
│   ├── 1-raw.md
│   ├── 2-typo-fixes.md
│   ├── 3-restructured.md
│   └── ...
├── versions.json
└── VERSION_CONTROL.md
```

### `iterations/`

Each version of the document lives as a separate file. Files are numbered sequentially and given a short descriptive suffix (e.g. `1-raw.md`, `2-typo-fixes.md`, `3-restructured.md`).

Every iteration is preserved in full — no version overwrites another.

### `versions.json`

A structured manifest tracking metadata for each iteration:

```json
{
  "title": "Document Title",
  "original_author": "Human author name",
  "iterations": [
    {
      "version": 1,
      "file": "iterations/1-raw.md",
      "description": "Brief description of this version",
      "edited_by": "Who made the edits (human name or AI model)",
      "ai_assisted": false,
      "changes": ["List of changes made"]
    }
  ]
}
```

#### Field definitions

| Field | Type | Description |
|-------|------|-------------|
| `title` | string | Title of the piece |
| `original_author` | string | The human who wrote the original draft |
| `version` | number | Sequential version number |
| `file` | string | Relative path to the iteration file |
| `description` | string | Brief summary of what this version represents |
| `edited_by` | string | Who made the edits — the person or AI that performed the changes, not the original author |
| `ai_assisted` | boolean | Whether AI was involved in producing this version |
| `changes` | array | List of specific changes made in this iteration |

## Conventions

- **`edited_by` reflects who made the change**, not who originated the piece. If Claude fixes typos, Claude is the editor. If the human restructures paragraphs, the human is the editor.
- **`original_author`** at the top level always credits the human creator.
- **`ai_assisted`** is `true` whenever an AI model contributed to the edits, even for minor changes like spellchecking.
- When AI is the editor, include the model name (e.g. `"Claude (Opus 4.6)"`).
- Keep `description` short — a phrase, not a paragraph.
- `changes` is optional for v1 (the raw draft) but recommended for all subsequent versions.

## Reuse

To use this system in a new writing project:

1. Create an `iterations/` folder
2. Save your first draft as `iterations/1-raw.md`
3. Copy the `versions.json` structure above and fill in your details
4. Each time the document is edited, save a new numbered file and add an entry to `versions.json`

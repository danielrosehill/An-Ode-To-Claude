Record a new iteration in versions.json.

Instructions:
1. Read the current `versions.json` to determine the next version number.
2. Check `iterations/` for the new file matching that version number (e.g. `4.md`, `5.md`).
3. If the file doesn't exist yet, ask the user which file to record.
4. Compare the new iteration against the previous one to identify what changed.
5. Ask the user to confirm who made the edits (default: the user, Daniel Rosehill). If the changes were made by Claude, record Claude as the editor. The `edited_by` field should reflect who actually performed the edits, not the original author.
6. Add a new entry to the `iterations` array in `versions.json` with:
   - `version`: next sequential number
   - `file`: relative path to the iteration file
   - `description`: brief summary of this version
   - `edited_by`: whoever made the changes
   - `ai_assisted`: true if Claude made the edits, false if the user did
   - `changes`: array of specific changes made

If the user provides context about what they changed (e.g. "I restructured the paragraphs and added a section about X"), use that to populate the description and changes fields. If not, diff the files to determine what changed.

$ARGUMENTS

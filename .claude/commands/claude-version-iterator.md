Create a new iteration of the essay based on the user's instructions.

CRITICAL RULES:
- ONLY make the changes the user has requested. Do not rewrite, rephrase, reorder, or "improve" anything else.
- Preserve all existing text VERBATIM except where the user's instructions specifically require changes.
- Do not fix typos, adjust formatting, add/remove punctuation, or clean up grammar unless explicitly asked.
- Do not move paragraphs or sections around unless explicitly asked.
- Maintain the exact same markdown structure (headings, links, italics, etc.) for all unchanged content.

Steps:
1. Read `versions.json` to find the current latest version number and its file path.
2. Read the latest iteration file.
3. Apply ONLY the changes described in the user's instructions below.
4. Write the result to `iterations/<next_version>.md` (e.g. if latest is `6.md`, write `7.md`).
5. Run `diff` between the old and new files to verify that only the requested changes were made. If unintended changes are found, fix them.
6. Update `versions.json` with the new iteration entry, including:
   - `version`: next sequential number
   - `file`: relative path to the new iteration file
   - `description`: brief summary of what was changed
   - `edited_by`: "Claude (Opus 4.6)"
   - `ai_assisted`: true
   - `changes`: array of specific changes made (derived from the user's instructions)

User's instructions for this iteration:
$ARGUMENTS

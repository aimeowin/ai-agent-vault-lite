# AGENTS.md — Universal agent instructions

You are an assistant working inside an Obsidian vault (plain Markdown files). Follow these rules.

## Read first
1. `60 Bot Memory/Profile.md` — who the user is (preferences, not secrets).
2. `60 Bot Memory/Active Context.md` — what's happening now.
3. `99 Meta/Conventions.md` — naming, tags, frontmatter.

## Writing rules
- Never delete notes. Move to `40 Archive/` only when asked.
- New captures → `00 Inbox/` with filename `YYYY-MM-DD HHmm <short title>.md`.
- Always add frontmatter: `type`, `created`, `tags`, `source: agent`.
- Use `[[wikilinks]]` to link existing notes; don't invent links to notes that don't exist.
- Append to memory files; don't rewrite history. Use the entry formats in `60 Bot Memory/README.md`.
- Keep facts and guesses separate: mark uncertain items with `(unverified)`.

## Never
- Store passwords, API keys, ID numbers, health or financial account data.
- Store information about other people beyond what the user explicitly provides.
- Edit files in `90 Templates/` or `50 Agents/` unless asked.

## End of every session
Append a session log to `60 Bot Memory/Session Log.md` (date, what was done, open loops).

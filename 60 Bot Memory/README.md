# Bot Memory — layout & formats
Agents read these files at the start of a session and append at the end.

| File | Contents | Write rule |
|---|---|---|
| `Profile.md` | Stable preferences (tone, tools, timezone) | Append; user approves edits |
| `Active Context.md` | Current focus, this week's priorities | Overwrite weekly |
| `Facts.md` | Durable facts | Append-only entries |
| `Decisions.md` | Decisions + rationale | Append-only |
| `Session Log.md` | One entry per agent session | Append-only |
| `Glossary.md` | Your terms & abbreviations | Append |

## Entry formats
Facts: `- YYYY-MM-DD | category | fact | confidence(high/med/low) | source`
Decisions: `### YYYY-MM-DD — Title` then `**Decision / Why / Alternatives / Revisit by**`
Session: `### YYYY-MM-DD HH:MM — agent name` then `Did / Changed files / Open loops`

## Privacy
Never store secrets, ID numbers, health/financial data, or details about other people.

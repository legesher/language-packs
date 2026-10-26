# AGENTS.md: working in language-packs

Context for AI coding assistants helping a contributor in this repository.

This is the contribution home for Legesher's language packs: the reviewing guide, the issue forms,
the reference templates (`reference/<tag>.md`, generated in the monorepo and mirrored here, never
edited by hand) and the submitted reviews (`reviews/`).

## The most common task: a native-speaker review by file

Follow [REVIEWING.md](REVIEWING.md), section 7, exactly. In short:

- Start from the language's template, `reference/<tag>.md`, copied to
  `reviews/<tag>/<tag>-<your-github-username>.md`. Never edit the template itself. In the
  copy, never edit the hidden first line or the `Key`, `English`, current-word and `Applies to`
  columns: the importer reads them.
- Keep the table structure: every row keeps its six cells (`Key`, `English`, the current word,
  `Applies to`, `Suggested`, `Comments`), one row per term. Verify the tables render.
- Row vocabulary: `✓` in Comments endorses; `Keep` plus a note endorses with a recorded limitation;
  a word in Suggested plus reasoning in Comments proposes a replacement; an untouched row is no
  opinion.
- Every suggestion needs reasoning. Where one change implies others (an `if`/`elif`/`else` family,
  a shared root across error names), keep the family consistent and say so.
- Language-wide observations go under "Notes for Future Updates", not in per-term cells.
- The consent block stays unchecked until the reviewer ticks it; never tick it for them. No email
  address goes in the file.
- One language per pull request; commits signed off (`git commit -s`); the pull request says AI
  assistance was used (see [AI_CONTRIBUTIONS.md](AI_CONTRIBUTIONS.md)).

## The agent's role

The human native speaker supplies the linguistic judgment; you supply everything around it. Do:
format tables, check cross-term consistency, verify markdown structure, look up what a Python
construct actually does, draft prose the reviewer edits. Do not: invent or improve translations
beyond what the reviewer decided, or fill review columns the reviewer has not worked through.

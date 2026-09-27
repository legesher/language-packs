# Community Guidelines

How we build together. This document sits alongside the [Code of Conduct](CODE_OF_CONDUCT.md): the
Code of Conduct covers how we treat each other, and these guidelines cover how we work on a shared
corpus of programming terminology without stepping on each other.

If you only read one section, read the next one.

## The shared corpus, and how disagreement works

Legesher collects every translation offered for every term as an option in a shared database. A
language pack is an export: the current best pick for each concept, chosen from the options that
exist so far. Most translation platforms converge on one locked string per term; we deliberately do
not. The options are the point. They are how a community works out, in the open, what its language
wants to call a concept.

That design carries a social contract:

- **Propose options; don't edit winners.** If a pack ships a word you would never use, the move is
  to offer your word and endorse the ones you agree with, not to overwrite the current pick. Your
  alternative is always a welcome contribution. It is never a conflict with a locked string, because
  nothing is locked.
- **A pick is a snapshot, not a verdict.** Today's export reflects today's endorsements. When better
  options arrive and native reviewers endorse them, the pick moves. Losing a round says nothing
  about the value of the word you offered.
- **Nothing is wasted.** Options that don't win stay in the corpus with their provenance and their
  endorsements. They inform style profiles, research, and future picks. The record is append-only
  on purpose. (Losing a ranking and failing moderation are different things: a submission the
  screen rejects for conduct or mechanical validity, with the reason cited, stays in the record
  but out of every export. Rankings never reject anything.)
- **Established beats invented, and coining is legitimate.** If your community's classrooms already
  have a word for a concept, that word carries the strongest claim. Where no native term exists
  anywhere, proposing one is how every language has always built its scientific vocabulary. Both
  are contributions; say which one you are making.

## Content standards for language contributions

Language packs end up in classrooms. Terms that are slurs, sexualized, degrading, or otherwise
unusable in a room full of students do not ship, in any language.

How that is enforced, in order:

1. **A maintainer screens every submission before it is visible.** Automated screening does not
   exist yet, and until it does the screen is a person reading each new word. Your contribution is
   recorded on arrival and is held back from rankings and from the published corpus until it has
   been read and cleared (the queue is walked weekly at minimum while volume is low). Being held is
   not a punishment and never removes your contribution from the record; it means it has not been
   read yet, or that it needs eyes the maintainer does not have.
2. **Native reviewers judge in context.** Words carry weight machines cannot see, in both
   directions: a term that looks innocuous can be a regional slur, and a term that pattern-matches
   badly can be perfectly ordinary. The judgment call belongs to people who live in the language.
3. **Everything is recorded.** Flags and their resolutions are append-only and visible on the
   option, so decisions can be understood and revisited rather than silently applied.

Conduct in comments, reviews, and discussions is covered by the Code of Conduct everywhere,
including its language-and-accessibility provisions. Dismissing a contribution because of the
language it is written in is a conduct issue here, not a difference of opinion.

## The moderation path

When something is flagged, whether by the screening gate or by a person:

1. A maintainer resolves the flag, with the resolution and reason recorded on the option.
2. A returned submission tells you exactly what to fix; a rejected one cites the guideline it
   failed.
3. Appeals follow the Code of Conduct's reporting and appeal path.

Moderation exists to keep the corpus trustworthy, and it is deliberately narrow: mechanical validity
and conduct are the only things that block. Creative disagreement is never a moderation matter.

## Style guides are suggestions

Each language accumulates a style profile: how compound words join, what stands in for uppercase
where a script has no case, how numerals read, what register docstrings take. These profiles guide
writers and tools, and they are always suggestions, never laws. A style profile describes how a
language community tends to write; it does not gatekeep what an individual is allowed to write.

## Where conversations happen

- **GitHub issues and pull requests** in this repository: the contribution forms and the
  [reviewer guide](REVIEWING.md) are the way in.
- **GitHub Discussions**, for questions, ideas, and anything that is not yet an issue.
- **Reviewer coordination** runs by email today: <contribute@legesher.com>, mentioning your
  language. Per-language channels come as native-review activity grows.

Thank you for being here. The community that forms around a language pack is the thing that makes
it real.

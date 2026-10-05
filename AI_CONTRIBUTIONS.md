# AI-Assisted Contributions

Legesher is a project about languages, built at a time when language models are part of how people work. We use AI in our own
workflow, and we expect many contributors will too. This guide explains what is welcome, what we ask of you, and which decisions stay with people.

## AI-assisted work is welcome

Unless an issue is labeled otherwise, AI-assisted work is welcome here.

What we ask is one line in your pull request saying so. The PR template has a spot for it. Something
like:

> AI-assisted: first draft generated with an assistant; I reviewed and tested every change.

That is all we ask. Declaring it is a courtesy to your reviewer: reviewers read
machine-drafted and hand-written code with different eyes, and knowing which they are looking at
makes review faster and kinder for everyone.

Two things follow from the declaration:

1. **You own correctness.** The DCO sign-off certifies the contribution is yours to give, and that
   includes standing behind what it does. If a reviewer asks why a line works the way it does, "the model wrote it" is not a complete answer. Take the time to understand
   what you submit.
2. **The quality floor does not move.** Tests, formatting, changelog, review: the same checks apply
   to every contribution regardless of how it was drafted. We review the work itself, however it was drafted.

## Labels that change this

### `ai:restricted`: do this one by hand

Some issues exist so that a person can learn a process by working through it by hand. When you see
`ai:restricted`, read it as an invitation: this issue is a good place to build real understanding,
and we would like you to have that.

This is an honor system. Nobody scans your commits or runs detectors on your prose. The check is the
review conversation itself, which works best when the person in it did the work. If you want the
issue but not the restriction, comment and ask; there is usually a sibling task where AI assistance
is fine.

### `ai:native-prompting`: use AI in your language

These issues ask you to use AI on purpose, in your own language: prompt in your heart language, use
your language pack's terms, and report what actually happens. Which surface to use is named on each
issue.

The observation is the contribution. Where the assistant understood you, where it drifted back to
English, which terms it refused to use: those reports feed the shared terminology corpus and our
research directly. No fix is expected from you. These issues are a good first contribution if you do not know where to start, and they help more than you might expect.

## Words proposed by models

The corpus keeps every word offered for every term as an option, with
provenance recorded: who or what proposed it, how, and when. Machine-suggested options are welcome
in that collection and are labeled as machine-provenance in the database. They compete on merit with
every other option.

Models review as well as propose (ranking, annotating, flagging things worth a human's attention),
and machine reviews are labeled as machine reviews everywhere they appear, carrying **zero weight
toward every promotion gate**. Where humans are counted, the [reviewer guide](REVIEWING.md) states
the exact rules: the `reviewed` tier counts native endorsements; the `official` gate's review depth
counts any screened human reviewer; and the act that promotes a pack (the convened ratification
session) is valid only with a quorum of verified native speakers.

One rule has no exceptions: **sign-off is human.** A model's proposal can enter the options and a
model's review can point people at problems, but no machine's opinion moves a term up the ladder or
ships a pack. AI drafts; people decide what their language ships with. What happens to the words
you contribute (credit, withdrawal, publication) is covered by
[the contributor notice](CONTRIBUTOR_PRIVACY.md).

## Summary

- AI may draft code, docs, words for the corpus, and tests. You review, run, and stand behind them.
- Declaration is one line in the PR, always.
- `ai:restricted` is an invitation to learn by hand, honored on trust.
- Sign-off is always human; machine reviews carry zero gate weight.

Questions about any of this belong in
[GitHub Discussions](https://github.com/legesher/legesher-translations/discussions). If a rule here reads as unclear or unkind, please tell us.

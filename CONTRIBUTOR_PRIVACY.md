# Your contributions and your data

**Version 1.0 · 2026-08-10**

When you offer a translation to Legesher, two things happen: your word joins a public research
corpus, and a record that *you* offered it exists in our database. This document explains both,
because you should be able to decide about them separately.

It sits alongside the [Community Guidelines](COMMUNITY_GUIDELINES.md), which cover how we work
together, and [CONTRIBUTING.md](CONTRIBUTING.md), which covers how to submit. This one covers what
happens to your work and to you afterwards.

If you only read one thing: **your word is published, your name is not, unless you ask for it to
be.**

## What happens to a word you offer

Legesher keeps every translation anyone has ever proposed for a programming term, in a shared
database. Your submission becomes two records:

- **An option**: the word itself, the concept it renders, the language, and where it came from.
- **An endorsement**: a record that a person stood behind that word, which is what moves a
  language pack from experimental toward official.

Both are published in the **Legesher language corpus**, a public research dataset. This is the point
of the project: the corpus is how a community's own decisions about its programming vocabulary
become visible, citable, and reusable by people we will never meet: researchers, educators, and
other language projects.

The corpus is released under **[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)**. Anyone
may use it, including commercially, as long as they credit the source. We chose a permissive licence
deliberately: a corpus nobody may use is a corpus that helps nobody.

We do not sell community-contributed translation data. That commitment is in our
[public terms](https://www.legesher.io/terms), not just here.

> **Current status.** The corpus is public:
> [huggingface.co/datasets/legesher/language-corpus](https://huggingface.co/datasets/legesher/language-corpus),
> open to anyone without an account. Please contribute on the understanding that your word is
> readable by anyone, now and in every future release.

## How you are identified

You are not identified. In the published corpus you are a string like this:

```text
c_0123456789abcdef        # illustrative only, not a real contributor
```

That is a one-way cryptographic digest of your GitHub username, computed with a secret key that
never leaves our systems. It is stable, so your endorsements stay connected to each other over time,
and it is opaque, so nobody can work backwards from it to you.

Two consequences worth understanding:

- **The published corpus contains no names, handles, or email addresses.** Not obscured ones.
  None. If someone downloads the dataset, they can see that one contributor endorsed forty words in
  Amharic. They cannot tell who.
- **We hold the only mapping.** A private table connects your opaque id to your GitHub username,
  your contact address, and your credit preference. It is never exported, and the export tooling
  fails outright rather than include it.

## What we never publish

Beyond identity, some things are deliberately withheld:

| Not published | Why |
| --- | --- |
| The mapping from your id to you | It is the only route back to a person |
| Your email address | Collected so we can reach you; never distributed |
| Comments attached to your endorsement | Free text next to a vote can carry personal detail |
| Reviewer labels on individual words | Historical records that contain real first names |
| Moderation and harm reports | About words *and* the people who flagged them |
| Model reasoning text | Machine output, not your work, and not useful to publish |

## Credit

Credit is **opt-in**. By default you are anonymous, and staying anonymous costs you nothing: your
endorsements count exactly the same.

You may choose:

- **Anonymous** (the default): only the opaque id appears, anywhere.
- **Handle**: your GitHub handle may be shown where contributors are credited.
- **Name**: a display name you give us may be shown instead.

You may change this at any time by asking. Changing it forward is immediate; it does not rewrite
dataset revisions that were published before you changed it.

## Withdrawal

You may ask us to remove your personal data at any time, for any reason, without explaining why.

**What we do.** We erase every field that could identify you (the username your id was derived
from, your display name, your handle, your contact address) and record that a withdrawal happened
on that date. What remains is a row saying "this contributor withdrew," attached to an id that no
longer leads anywhere.

**What stays, and why.** Your endorsements remain in the corpus as anonymous evidence. This is
deliberate, and it is the one part of this policy we ask you to accept rather than choose:

- Other people's work depends on those counts. An endorsement is part of how a community reached a
  decision about a word. Removing it silently changes which word a language pack ships, for
  everyone.
- The record no longer says anything about *you*. Once the mapping is erased, an endorsement is a
  data point with no person attached.

If what you want is your *contributions* removed rather than your *identity*, say so. That is a
different request, we will discuss it with you, and we will not pretend it is the same thing.

**Why we keep an empty record instead of deleting the row.** Contributions arrive in batches that
carry your username. If we ever rebuild the database from those batches (after a bug, or to correct
a record, both of which happen), an importer that has no memory of your withdrawal would recreate
your identity from the batch and undo it. The withdrawal marker is what prevents that. It holds no
information about you; it exists only to make sure the erasure sticks.

**What withdrawal cannot do.** Two limits, stated plainly, because you would otherwise discover them
later:

- If you submitted through a public pull request or issue, that submission is part of a public
  repository's history under your own account. We cannot retroactively unpublish something you
  published yourself.
- Where your identity was recorded in our own repository, removing it is a commit, and the commits
  before it still contain it. Clearing repository history requires a rewrite, which we do at defined
  points rather than on demand. Ask us where that stands and we will tell you.

Withdrawal covers our database and our published datasets completely. It does not cover version
history, and we would rather say so than let "we deleted it" quietly mean less than you assumed.

**Coming back.** If you withdraw and later want to contribute again, just say so. We clear the
marker and record your consent afresh. It never happens automatically.

## How to ask

Any of these reaches a person:

- **Privacy, credit, or withdrawal requests**: <help@legesher.com>
- **Anything about contributing**: <hello@legesher.com>
- **General discussion**:
  [GitHub Discussions](https://github.com/legesher/language-packs/discussions)

You do not need to use particular wording. "Please remove me" is enough.

Your rights under GDPR, UK GDPR, and CCPA/CPRA apply to everything described here, including the
right to access what we hold about you and to lodge a complaint with your data protection
authority. The full enumeration lives in the
[company-wide Privacy Policy](https://www.legesher.io/privacy).

## Changes to this document

This notice is versioned, and the version you agreed to is recorded with your consent. If we change
what we do with contributor data in any way that matters, we publish a new version and record the
change here. We do not quietly amend the old one.

| Version | Date | Change |
| --- | --- | --- |
| 1.0 | 2026-08-10 | First published. Governs contributions made from this date. |
| `oss-pre-notice` | before 2026-08-10 | Not a version of this notice. See below. |

**If your consent is recorded as `oss-pre-notice`,** it means you contributed
before this notice existed: through a public pull request under your own
account, credited by handle in the language pack changelogs at the time. We
record that rather than leaving it blank, because leaving it blank would say
nobody ever agreed to anything, and recording `1.0` would claim you accepted a
document that did not exist.

It grants us nothing. You are anonymous by default like everyone else, and
withdrawal works for you exactly as described above. If you would like to be
credited, or to be covered by this notice going forward, tell us and we will
record it.

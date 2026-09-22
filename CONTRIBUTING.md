# Contributing

This repository is the home of translation contribution for Legesher: the place a word you would
teach becomes part of the shared corpus. Everything here is built so that a linguist, a teacher, or a
careful reader can contribute without knowing git — and so that a developer can go deeper when they
want to.

## The ways in

1. **Offer a single word** — the
   [propose form](https://github.com/legesher/legesher-translations/issues/new?template=propose_translation.yml).
   One term, your word, your reasoning. No account needed beyond GitHub.
2. **Review a pack in bulk** — the
   [bulk review form](https://github.com/legesher/legesher-translations/issues/new?template=language_pack_review.yml)
   takes many terms in one issue.
3. **Run a full review session by file** — produce a review bundle and submit it by pull request.
   The [reviewer guide](REVIEWING.md) explains the kit, the bundle, and the lane.
4. **Sign up as a reviewer** — the
   [signup form](https://github.com/legesher/legesher-translations/issues/new?template=reviewer_signup.yml)
   tells us your language and how you would like to be credited.
5. **Flag a term** — the
   [feedback form](https://github.com/legesher/legesher-translations/issues/new?template=pack_feedback.yml)
   for real problems: harmful, wrong in meaning, wrong register, or spam.

Start with the [reviewer guide](REVIEWING.md) — it covers the whole journey, from your word to a
shipped pack. The [Community Guidelines](COMMUNITY_GUIDELINES.md) carry the social contract
(options, not winners), [AI-Assisted Contributions](AI_CONTRIBUTIONS.md) says how AI use works
here, and [Your contributions and your data](CONTRIBUTOR_PRIVACY.md) is the notice every
submission asks you to agree to.

## What happens to a submission

A person reads it first — every submission is screened by a maintainer before it becomes visible
or exported (the queue is walked weekly at minimum). Your issue is then closed with a reply naming
exactly what landed. Cleared words join the public
[language corpus](https://huggingface.co/datasets/legesher/language-corpus); endorsements
accumulate there; packs re-release when a language crosses a promotion gate. Nothing you submit
edits a shipped pack directly — that decoupling is what lets review stay open to everyone.

## Contributing to this repository itself

Improvements to the docs, the forms, and the review tooling in this repo are welcome as ordinary
pull requests. Two things apply:

- **The pack trees and generated files are not hand-edited.** Generated content arrives through
  maintainer tooling with a build manifest; a wrong word is fixed through review, never by editing
  an artifact. If a file's header says it is generated, propose the change through the forms
  instead.
- **AI-assisted work is welcome and declared** — one line in your PR, per
  [AI-Assisted Contributions](AI_CONTRIBUTIONS.md).

## Developer Certificate of Origin (DCO)

Pull requests certify the [Developer Certificate of Origin](https://developercertificate.org/):
by signing off, you attest the contribution is yours to give under this repository's license. Add
the sign-off to each commit:

```bash
git commit -s -m "your message"
```

which appends a `Signed-off-by: Your Name <your@email>` line. The issue-form lanes have no commit
to sign; there, the consent box you tick records the same attestation together with the notice
version you agreed to.

## Questions

- Anything about contributing: <contribute@legesher.com>
- Privacy, credit, or withdrawal: <privacy@legesher.com>
- Conduct: <conduct@legesher.com> — the [Code of Conduct](CODE_OF_CONDUCT.md) applies everywhere
  here, including its language-and-accessibility provisions.

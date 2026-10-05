# Contributing

Thank you for being here. This repository is where Legesher's language packs are localized, and you
can contribute without knowing how to code or how to use git. If you are a developer, there are ways
to go deeper too.

## Ways to contribute

1. **Share a word.** Use the [propose form](https://github.com/legesher/legesher-translations/issues/new?template=propose_translation.yml)
   to offer your word for one term and tell us why you chose it. All you need is a GitHub account.
2. **Review many terms at once.** The
   [bulk review form](https://github.com/legesher/legesher-translations/issues/new?template=language_pack_review.yml)
   takes many terms in one issue.
3. **Review by file.** For a full review session, create a review bundle and submit it as a pull
   request. The [reviewing guide](REVIEWING.md#7-reviewing-by-file) explains how.
4. **Sign up as a reviewer.** The
   [signup form](https://github.com/legesher/legesher-translations/issues/new?template=reviewer_signup.yml)
   asks for your language and how you would like to be credited.
5. **Flag a term.** Use the
   [feedback form](https://github.com/legesher/legesher-translations/issues/new?template=pack_feedback.yml)
   when a term is harmful, wrong in meaning, in the wrong register, or spam.

If you are new, start with the [reviewing guide](REVIEWING.md). It explains the whole process, from
the word you offer to a released pack.

## Before you contribute

Please read these first:

- [Community Guidelines](COMMUNITY_GUIDELINES.md): how we work together and how disagreement is
  handled.
- [AI-Assisted Contributions](AI_CONTRIBUTIONS.md): how to use AI in your contributions.
- [Your contributions and your data](CONTRIBUTOR_PRIVACY.md): the notice every submission asks you
  to agree to.
- [Code of Conduct](CODE_OF_CONDUCT.md): how we treat each other.

## What happens to a submission

1. A maintainer reads every submission before it is shown to anyone else or exported.
2. Your issue is closed with a reply that tells you exactly what was added.
3. Cleared words are added to the public
   [language corpus](https://huggingface.co/datasets/legesher/language-corpus), where reviewers
   endorse the words they would teach.
4. When a language has enough review, its pack is released again.

A submission never edits a released pack directly. Packs are built from the corpus, so a word is
changed through review.

## Changes to this repository

Improvements to the documentation, the forms, and the review tooling are welcome as pull requests.
Two things to know:

- **Generated files are not edited by hand.** Pack files and other generated content are built by
  maintainer tooling. If a file's header says it is generated, propose your change through the
  forms.
- **Tell us when you used AI.** One line in your pull request is enough. See
  [AI-Assisted Contributions](AI_CONTRIBUTIONS.md).

## Developer Certificate of Origin (DCO)

Pull requests certify the [Developer Certificate of Origin](https://developercertificate.org/). By
signing off, you confirm the contribution is yours to give under this repository's license. Add the
sign-off to each commit:

```bash
git commit -s -m "your message"
```

This adds a `Signed-off-by: Your Name <your@email>` line. The issue forms have no commit to sign.
There, the consent box you tick records the same confirmation, together with the version of the
notice you agreed to.

## Questions

- Contributing: <contribute@legesher.com>
- Privacy, credit, or withdrawal: <privacy@legesher.com>
- Conduct: <conduct@legesher.com>

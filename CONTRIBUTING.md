# Contributing

Thank you for being here. This repository is where Legesher's language packs are localized into
your heart language to reflect the beautiful depth hidden within language.

## Pathways

There is one way to contribute today, built for people comfortable with GitHub.

**Review a language pack by pull request.** Copy your language's template, `reference/<tag>.md`,
to `reviews/<tag>/<tag>-<your-github-username>.md`, work through the terms, tick the Required
boxes, and open a pull request. The
[reviewing guide](REVIEWING.md#start-here-review-by-pull-request) walks through each step, and
[section 7](REVIEWING.md#7-reviewing-by-file) covers the file in detail.

If a current word is harmful or wrong in meaning and you have no replacement to offer, say so in the
Comments column of your review, or write to <contribute@legesher.com>.

More ways to contribute are coming. To ask for a language that has no pack yet, use the
[new language request](https://github.com/legesher/legesher/issues/new?template=add_language.yml).

## Before you contribute

Please read these first:

- [Community Guidelines](COMMUNITY_GUIDELINES.md): how we work together and how disagreement is
  handled.
- [AI-Assisted Contributions](AI_CONTRIBUTIONS.md): how to use AI in your contributions.
- [Your contributions and your data](CONTRIBUTOR_PRIVACY.md): the notice every submission asks you
  to agree to.
- [Code of Conduct](CODE_OF_CONDUCT.md): how we treat each other.

## What happens to a submission

1. The review check runs on your pull request, and a maintainer reads every line before anything is
   shown to anyone else or exported.
2. Within 7 days, a maintainer replies on the pull request: either it is ready to merge, or the reply
   names exactly what to fix. Push fixes to the same branch, with each commit signed off.
3. After the merge, your endorsements and suggestions are added to the public
   [language corpus](https://huggingface.co/datasets/legesher/language-corpus). A new word you
   suggest is held until a maintainer clears it.
4. When a language has enough review, its pack is released again.

Your review file, comments included, is public in this repository once merged, so never put an
email address or private contact detail in it.

A submission never edits a released pack directly. Packs are built from the corpus, so a word is
changed through review.

## Changes to this repository

Improvements to the documentation and the review tooling are welcome as pull requests.
Two things to know:

- **Generated files are not edited by hand.** Pack files and other generated content are built by
  maintainer tooling. If a file's header says it is generated, propose your change in a review
  instead.
- **Tell us when you used AI.** One line in your pull request is enough. See
  [AI-Assisted Contributions](AI_CONTRIBUTIONS.md).

## Developer Certificate of Origin (DCO)

Pull requests certify the [Developer Certificate of Origin](https://developercertificate.org/). By
signing off, you confirm the contribution is yours to give under this repository's license. Add the
sign-off to each commit:

```bash
git commit -s -m "your message"
```

This adds a `Signed-off-by: Your Name <your@email>` line. If you already made a commit without it,
add the sign-off and update your branch:

```bash
git commit --amend -s --no-edit
git push --force-with-lease
```

In a review file, the Required box for the Developer Certificate of Origin records the same
confirmation, together with the version of the contributor notice you agreed to.

## Questions

- Contributing: <contribute@legesher.com>
- Privacy, credit, or withdrawal: <privacy@legesher.com>
- Conduct: <support@legesher.com>

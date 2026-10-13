# Incoming review bundles

Review bundles are submitted to this folder. A bundle is one JSON file for one review session, in
the format the bundle schema defines (the schema ships with the `legesher-i18n` package). The
[reviewing guide](../../REVIEWING.md#7-reviewing-by-file) explains how to create one.

## How to submit a bundle

1. Add your bundle at `reviews/incoming/<your-language>/<anything>.json` and open a pull request.
2. Checks report schema and validation results on the pull request. While the checks are being set
   up, a maintainer runs the same validation by hand, which takes a little longer.
3. A maintainer reviews the bundle. When the pull request is merged, your review is accepted and
   goes through the same import, screening, and corpus steps as every other contribution.

## Rules

- **A bundle is public.** Never put an email address or private contact detail in one. To reach us
  privately, write to <hello@legesher.com>.
- **Merged bundles are not edited.** They are the record of what was accepted. To correct a review,
  submit a new session.

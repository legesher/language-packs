# Reviews

Reviews are submitted to this folder by pull request, one file per review session, in one of two
formats. The [reviewing guide](../../REVIEWING.md#7-reviewing-by-file) explains both.

- **A markdown review**: your language's reference template (`reference/<tag>.md`) with the
  Suggested and Comments columns filled in.
- **A JSON bundle**: one file in the format the bundle schema defines (the schema ships with the
  `legesher-i18n` package).

## How to submit

1. Add your file under `reviews/<tag>/`, where `<tag>` is your language's BCP 47 tag, the
   name of its template under `reference/`. A markdown review is named
   `<tag>-<your-github-username>.md`; after a pack version bump, a new review is
   `<tag>-<your-github-username>-<pack-version>.md`. A bundle is `<anything>.json`.
2. Open a pull request. Checks report schema and validation results on the pull request. While the
   checks are being set up, a maintainer runs the same validation by hand, which takes a little
   longer.
3. A maintainer reviews the file. When the pull request is merged, your review is accepted and goes
   through the same import, screening, and corpus steps as every other contribution.

## Rules

- **A review file is public.** Never put an email address or private contact detail in one. To
  reach us privately, write to <contribute@legesher.com>.
- **The username in a markdown review's file name must be the account that opens the pull
  request.** The importer takes your identity from the pull request, not from the file.
- **A markdown review is pinned to the pack version its template names.** A second review of the
  same pack version updates your existing file in a new pull request. After a pack version bump,
  start a new file from the regenerated template; the old file stays as it was accepted.
- **Merged bundles are not edited.** A JSON bundle is the record of one session. To correct one,
  submit a new session.

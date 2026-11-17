# Reviews

Reviews are submitted to this folder by pull request, one file per review session: your language's
reference template (`reference/<tag>.md`) with the Suggested and Comments columns filled in. The
[reviewing guide](../REVIEWING.md#start-here-review-by-pull-request) explains each step, and
[section 7](../REVIEWING.md#7-reviewing-by-file) covers the file in detail.

## How to submit

1. Add your file under `reviews/<tag>/`, where `<tag>` is your language's BCP 47 tag, the
   name of its template under `reference/`. Name it `<tag>-<your-github-username>.md`; after a pack
   version bump, a new review is `<tag>-<your-github-username>-<pack-version>.md`.
2. Fill in "About you", tick the Required boxes under "Before you submit", and keep one choice on
   the "Credit me as" line.
3. Open a pull request, each commit signed off. Checks report validation results on the pull
   request. While the checks are being set up, a maintainer runs the same validation by hand.
4. A maintainer replies within 7 days. When the pull request is merged, your review is accepted and
   goes through the same import, screening, and corpus steps as every other contribution.

## Rules

- **A review file is public.** Never put an email address or private contact detail in one. To
  reach us privately, write to <contribute@legesher.com>.
- **The username in the file name must be the account that opens the pull request.** The importer takes your identity from the pull request, not from the file.
- **A review is pinned to the pack version its template names.** A second review of the
  same pack version updates your existing file in a new pull request. After a pack version bump,
  start a new file from the regenerated template; the old file stays as it was accepted.

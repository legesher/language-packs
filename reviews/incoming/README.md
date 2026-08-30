# Review bundles, incoming

This is the landing lane for **review bundles**: one JSON file per review session, in the shape the
bundle schema defines (it ships with the `legesher-i18n` package). The
[reviewer guide](../../REVIEWING.md#7-review-sessions-by-file-the-bundle-lane) explains the kit,
the bundle, and the whole journey.

How the lane works:

1. Add your bundle at `reviews/incoming/<your-language>/<anything>.json` and open a pull request.
2. Checks annotate the PR with schema and mechanical results. (While the checks are being wired,
   a maintainer runs the same validation by hand — the result is the same, a little slower.)
3. A maintainer does the human screen, and **merging means your evidence is accepted**: it enters
   the same import, screening, and corpus path as every other lane.

Two rules protect everyone:

- **A bundle is a public artifact.** No email address or private contact detail ever goes in one —
  contact travels <contribute@legesher.com>.
- Merged bundles are the record of what was accepted; they are archived and imported, never edited
  in place. A correction is a new session, not a rewrite.

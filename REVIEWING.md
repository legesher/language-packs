# Reviewing a language pack

Legesher language packs let people write and read code in their heart language. Every pack starts
**experimental**: a machine proposed every word, and mechanical checks are all it has passed. A pack
becomes something better only through review by people who actually speak the language.

When you review a pack, you are an open-source contributor to Legesher, and you are credited like any other contributor.

This guide is written for linguists, teachers, and careful readers as well as developers. You do not need to know Python to review a Python pack. Everything here is a suggestion based on what tends to work.

**Get started:**
[sign up as a reviewer](https://github.com/legesher/language-packs/issues/new?template=reviewer_signup.yml),
[offer a single word](https://github.com/legesher/language-packs/issues/new?template=propose_translation.yml), or
[review a pack in bulk](https://github.com/legesher/language-packs/issues/new?template=language_pack_review.yml).

---

## 1. How to choose a word

Ask yourself: **if computer science had been born in your language, how would this concept be
taught?** What would the textbook call it? Localize the concept, not the English word. We are looking for the word your language would have chosen on its own.

In practice:

- **Established terms win.** If your community's classrooms already have a word for *division by
  zero* or *loop*, that word beats anything a model proposes. Tell us it is established. That is
  evidence.
- **Coining is legitimate.** Many concepts (*deprecation*, *generator*) have no native term anywhere
  yet. Proposing one is welcome. It is how every language built its scientific vocabulary. We
  follow the spirit of ISO 704: name the concept by its essential characteristics.
- **Genuine loanwords are yours too.** If your language really says «كمبيوتر» or "computer", keeping it is a valid choice for a native speaker to make. Mark it as a loanword or cognate.
- **Transliteration is allowed when it is labeled.** A sound-copy of the English word is usually a shortcut, and our models are not allowed to propose one. But if a phonetic borrowing
  is genuinely what your community uses and prefers, you may submit or endorse it. Tag it *transliteration* so the preference is visible. If most reviewers of your language
  prefer transliterated terms, that pattern becomes part of your language's recorded terminology
  policy.
- **Phrases get two answers.** For compound tokens (`elif` is "else if"), first agree how the *idea*
  reads in full in your language, then how it contracts into a single token. Both matter. The full phrase is what people learn from, and the short token is what ships.

## 2. If you have used Crowdin or Weblate

Welcome. Most of what you know carries over. One thing is different.

**What is the same:** strings keyed to source concepts, review with definitions and context in view,
credit for your work, a ladder of trust that weighs experienced reviewers more.

**What is different:** platforms like Crowdin and Weblate converge every string to one source-of-truth
translation, because a UI string must render one way. Legesher keeps every word offered as an option, because terminology is something a community works out over time. No string is locked, so there are no conflicts to resolve. Offer your word, endorse the ones you would teach, and rank them. The pack uses the current pick, and the words that were not picked stay in the record.

**How the terms map:** suggest a translation → propose an option · vote → endorse and rank ·
translation memory → the options table, with provenance · proofread step → native review ·
glossary lock → there is not one. The current pick can change.

## 3. What you can contribute

1. **Reserved words** (the priority): keywords, builtins, and exceptions, about 180 concepts for
   Python. Because packs are concept-keyed, your review of `break` ships in every programming
   language that has `break`.
2. **Error messages and common phrases**: the messages people see most, first. Placeholders are
   preserved, and the original is always shown alongside.
3. **Style profile**: how code should *read* in your language. How compound words join, what
   replaces UPPERCASE for constants where your script has no case, adjective and noun order in
   compounds, digit policy, docstring register. Your answers become your language's style guide,
   which is always a suggestion for writers, never a law.

Beyond the chosen words, your comments are collected too: how you would explain a concept to a
student, how words should be formed, notes on register. They go into the open terminology corpus
with your credit preference honoured, and they outlive any single term. Everything you write is kept, including words that are not picked.

## 4. Who can review

Anyone may submit. Endorsements are weighted by rung:

| rung | how you get there | what it carries |
| --- | --- | --- |
| anonymous | no account | recorded, weighted zero |
| contributor | signed-in contributor | counted, low weight |
| native (claimed) | you tell us this is your language when you sign up | counts toward `reviewed` |
| native (verified) | vouched by an existing verified reviewer of your language, a short verification call with a maintainer, or institutional affiliation as a teacher or linguist | full native weight; counts toward the quorum that promotes a pack |
| certified | credentialed engagements through the education work (see §10) | highest |
| maintainer | Legesher maintainers | equal to certified. On what a word means in your language, a maintainer does not outrank a certified native speaker |

Verification changes how much your endorsement counts. It does not change whether you are welcome. Claimed reviewers do full
reviews, and verification can come afterwards.

One detail to know: each endorsement carries the rung you held **at the moment you made it**. That
snapshot is permanent evidence and is not silently rewritten when you level up. Your earlier work is
never lost, but carrying your new weight will take a deliberate re-affirmation rather than happening
retroactively; the review app will offer that in one step once it ships.

## 5. What reviewing looks like

Today reviewing happens through GitHub issue forms. They need only a GitHub account and nothing installed. A richer review surface is being built on the
same store and the same rules, including one that does not assume you know git and works properly
for right-to-left scripts. The forms are the starting point, and they will keep working.

**We ask for your word first.** The most valuable signal a corpus can hold is the word a fluent
speaker reaches for *before* seeing anyone else's answer. Once you have seen a machine's confident
suggestion, you cannot un-see it. So the propose form asks for your rendering without showing you
the current pick, and the review app will do the same for every term. The bulk review form is the
exception, because you are reading the shipped pack: those answers are recorded as responses to
candidates rather than as first instincts, and both are kept, distinctly.

**Endorse, pass, or flag (and rank, tag, comment).** Endorse every word you would genuinely teach,
including words other people proposed. Rank your endorsements: slot 1 means "ship this". Tag
descriptors such as transliteration, loanword, established, coinage, region, or register. Passing on
a word is always allowed and means "no opinion". It is never held against the word or against you.
(On the bulk review form these read as ✅ = endorse, ❓ = offer an alternative, 🤔 = a comment worth
keeping.)

**There are no downvotes.** Disagree by endorsing a better word, or by proposing one. A
[flag](https://github.com/legesher/language-packs/issues/new?template=pack_feedback.yml) is reserved for real problems (harmful,
wrong in meaning, wrong register, spam) and asks for a sentence of explanation. A person reads every flag. Flags do not change a score.

**Partial reviews are welcome.** Thirty concepts reviewed carefully are worth more than 180 reviewed in a hurry.

**Models review too, and their reviews carry no weight.** We use language models to propose candidates,
and we also let them review: ranking, annotating, flagging things worth a human's attention. Machine
reviews are labeled as machine reviews everywhere they appear, and they carry **zero weight toward
every gate below**. `Reviewed` means native speakers; a model can never be one of them. A model's
flag routes to a person and rejects nothing on its own.

## 6. Where your contribution goes

Step by step:

1. **You submit**: a form, or a review session by pull request (§7).
2. **A person reads it.** Every submission is held until a maintainer has screened it (§12). Your
   issue will be **closed with a reply** naming exactly what landed. Closed means *recorded*, never
   rejected. A submission that cannot be cleared yet is either **held** (usually: waiting for a
   native reviewer of your language to exist) or **returned or rejected with the reason cited**. A
   held submission stays out of sight until a reviewer can look at it. A held submission is not cleared by time passing. It needs a reviewer.
3. **Cleared words join the corpus.** The evidence lives in
   [`legesher/language-corpus`](https://huggingface.co/datasets/legesher/language-corpus) on
   Hugging Face: every candidate rendering and every endorsement, under CC BY 4.0, with
   contributors as opaque ids. See your language's evidence yourself:

   ```python
   from datasets import load_dataset
   options = load_dataset("legesher/language-corpus", "options")
   ```

4. **Endorsements accumulate; gates release.** Nothing you do edits a shipped pack directly. When a
   language crosses a gate (§9), the pick is re-cut from the evidence and a new pack version ships.
   The words that were not picked stay in the corpus.

## 7. Reviewing by file

For a full session over many terms, a file works better than the forms: take the **review kit** for your
language (terms, candidates, and context, deliberately without anyone else's verdicts), record your
endorsements, passes, flags, rankings, and your own renderings, and produce a **bundle**: a single
JSON file in the shape the bundle schema defines (it ships with the `legesher-i18n` package). A
review app that walks the kit and writes the bundle for you is being built; writing it by hand or
by script works today.

Submit the bundle as a pull request into `reviews/incoming/<your-language>/`. Checks annotate the
PR with schema and mechanical results; a maintainer does the human screen; **merging means your
evidence is accepted** and goes through the same import, screening, and corpus steps as every other contribution.
Until the incoming directory and its checks are live, attach the bundle file to a
[bulk review issue](https://github.com/legesher/language-packs/issues/new?template=language_pack_review.yml)
instead. It is handled the same way.

One rule: **a bundle is public.** Never put an email address or private contact detail in one. To reach us privately, see §11.

## 8. What blocks a submission

Only these block a submission:

- **Valid identifiers.** Terms must be valid identifiers: no spaces or punctuation, stable under
  Unicode NFKC normalization, consistent script, no invisible characters. A failing term is kept as
  evidence but cannot ship.
- **Round-trip.** Two different concepts cannot share one word within your language, because code has to convert back to its original form without loss.
- **Placeholders.** In the messages track, `{name}`-style placeholders must survive, though you may
  reorder them.
- **Conduct.** Submissions pass the [Code of Conduct](CODE_OF_CONDUCT.md), including its
  language-and-accessibility provisions. Harassment, slurs, or personal information in comments
  return or reject a submission.

These never block a submission:

- **Disagreeing with a model.** Model output is a starting point. It has no authority. Multilingual models
  underperform in exactly the languages we care most about, and your judgment is the point of this
  process.
- **Novel coinages.** A word nobody proposed before routes to more human review, never to machine
  rejection.
- **Transliteration tags, register choices, or any style preference.**

## 9. How packs become official

| status | meaning | criteria |
| --- | --- | --- |
| **experimental** | ships now, labeled experimental | mechanical gates pass; no native review required, because review is iterative and never blocks availability |
| **reviewed** | native speakers have signed off | at least 2 native endorsements on each covered term, across at least 80% of the surface; no open flags |
| **official** | the certified tier | every term carries at least 10 reviews, and the shipped pick holds a majority of reviewers' first-choice rankings; style profile ratified; zero open flags; and a convened session of the language's reviewers ratifies the pack |

Each reviewer's top-ranked option counts as their one vote for a term, so "majority" always has a
plain denominator: the people who reviewed it. These criteria are arithmetic over the public corpus:
every endorsement they count is published, so anyone can recompute and check the numbers. A status page that does the arithmetic for you is planned.

The ten reviews are open to **any screened reviewer**, not only verified natives. We do not want verification to slow participation, so the requirement for verified native speakers applies at the ratification session.

**A pack becomes official in a meeting.** Reaching the numbers makes a pack eligible. Official status is conferred in a
convened ratification session of the language's reviewers, which reads the evidence, can override
the computed majority for reasons it records, and is valid only with a quorum of verified native
speakers present: at least three of them, or a majority of those attending, whichever is greater.
The numbers decide when a pack is *eligible*. The session decides whether it is ready.

One consequence: a language community that cannot yet field ten reviewers cannot reach
official. That is intentional. There is no scaled-down threshold and no maintainer override, because
`official` is a claim made to strangers choosing a curriculum or adopting a vocabulary, and it has to mean the same thing in every language. A pack stays at `reviewed`, fully usable and labeled as such, until its community reaches that size. The requirement is about how many people have reviewed the pack. It is not a judgment of the language.

Packs can move down as well as up: a verified defect returns a term to experimental until
re-reviewed. Nothing is deleted. Every submitted word and comment remains part of the record, and
your identity remains withdrawable (§11).

## 10. Recognition

- **Credit.** With every submission you choose how public credit reads: **anonymous** (an
  opaque contributor id, and the default), **your handle**, or **a display name you give us**.
  Whatever you pick appears, or does not, wherever contributors are credited. You can change the
  choice later by asking. Your endorsements count identically in every case.
- **Founding reviewers.** The first verified native reviewers to carry a language to `reviewed` are
  recorded as such, permanently.
- **Reach.** Concept-keyed review means your work ships across programming languages: a review of
  `break` lands in every pack that has one.
- **Paid review work.** Reviewing here is volunteer open-source contribution. Legesher's
  education work will engage fair-wage reviewers for course-edition and accreditation projects, and
  verified reviewers from this program are the natural candidates when those engagements exist. One does not require the other, and volunteering here does not mean your expertise has no value.

## 11. Licensing, attribution, and your data

- Words and comments you submit ship inside the Apache-2.0 language packs and are published in the
  public research corpus under CC BY 4.0. On the pull-request lane your commits carry a
  [DCO sign-off](CONTRIBUTING.md#developer-certificate-of-origin-dco) attesting the work is yours to
  give; on the issue-form lanes there is no sign-off step. The consent box you tick records the
  same attestation together with the notice version.
- The published corpus credits you by opaque contributor id, plus your chosen credit where you chose
  one. Your identity details are never part of the published dataset, and you may withdraw at any
  time: counts survive, your personal data does not.
- **We never ask for your email on a public form.** GitHub issues are public, so contact details
  travel a private channel instead: write to <contribute@legesher.com> and mention your issue. An
  address given that way is stored privately alongside your identity, never in the repository, never
  in the dataset, and deleted with the rest of your identity if you withdraw.
- Terms shown from other projects appear with attribution. Endorsing one records *your* independent
  judgment of that word.
- **Your contributions may appear in research.** The open corpus is research data by design, and we
  may publish analyses of it. Your identity and private session details are never part of that.
- **Published dataset versions are permanent.** Withdrawal removes your identity everywhere and stops
  your words appearing in *future* releases, but versions already published and downloaded cannot be
  recalled. We want you to know this before you contribute.

The full account is in [Your contributions and your data](CONTRIBUTOR_PRIVACY.md), the notice
each submission asks you to agree to. It is versioned, and the version you agreed to is recorded
with your consent, so a later revision re-consents naturally on your next contribution rather than
applying to you retroactively.

## 12. Screening, moderation, and appeals

**A person reads your submission before it goes anywhere.** Everything a stranger submits is held
until a maintainer has looked at it: mechanical validators run first, and then a human judges the
rendering itself before it becomes visible to other reviewers or exported to the corpus. The queue
is walked weekly at minimum while volume is low.

An automated screening step is being built, and this guide will say so when it ships. Today a maintainer does the screening.

Flags and conduct screens are resolved by maintainers, recorded append-only, with the resolution
visible on the option. A returned submission tells you exactly why and how to fix it; a rejected one
cites the guideline. Appeals follow the [Code of Conduct](CODE_OF_CONDUCT.md)'s appeal path.

## Questions

- **Anything about contributing**: <contribute@legesher.com>
- **Privacy, credit, or withdrawal**: <privacy@legesher.com>
- **Conduct**: <conduct@legesher.com>
- **Everything else**:
  [GitHub Discussions](https://github.com/legesher/language-packs/discussions)

If something here reads as unclear or unkind, please tell us.

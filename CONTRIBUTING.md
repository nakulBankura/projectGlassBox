# Contributing

Thanks for helping. This is an open research project on transparent, verifiable elections for India. You don't need to be a cryptographer to contribute. Critical reading, prior-art research, usability thinking and clear writing all matter.

## Ways to contribute

- **Challenge the threat model.** Read `docs/threat-model.md` and point out missing attackers, wrong assumptions or unclear properties. This is the most valuable contribution right now.
- **Work on an open problem.** Pick an issue labelled `open-problem` and share your analysis, references or a proposal.
- **Add prior art.** Summarise a paper, system or report in `research/` (a short summary with a link is enough).
- **Improve documentation.** Fix errors, clarify wording, add translations.
- **Review.** Comment on other people's proposals and pull requests.

## Ground rules

1. **Stay non-partisan.** No discussion of parties, candidates or specific election results.
2. **No overclaiming.** Say what a design does and does not protect against. Do not describe anything as "unhackable" or "corruption-proof".
3. **Cite your sources.** Link papers, standards or reports for technical claims.
4. **State your assumptions.** Every proposal should list what it trusts.
5. **Be kind and specific.** Critique ideas, not people. See `CODE_OF_CONDUCT.md`.

## How to propose a change

1. **Small fixes** (typos, links, clarity): open a pull request directly.
2. **Anything bigger** (new design, changed requirement, new protocol idea): open an issue or a Discussion first so others can respond before you invest time.
3. **Design decisions:** once a decision is agreed, record it as a short file in `docs/decisions/` with the context, the options considered and the reasoning.

## Pull requests

- Fork the repo, make a branch, and open a pull request against `main`.
- Keep each pull request focused on one topic.
- Describe what changed and why. Link the related issue if there is one.
- Expect review comments. Changes to the threat model or requirements need discussion before merging.

## Security issues

If you find a vulnerability in anything in this repo, do not open a public issue. Follow the steps in `SECURITY.md`.

## Licensing

By contributing, you agree that your contributions are licensed under the project's licenses: Apache-2.0 for code and CC BY 4.0 for documentation.

# [Project GlassBox]

Open research on transparent, verifiable elections for India.

> **Status: early-stage research.** This is not a working, audited, or secure voting system. It is not affiliated with or endorsed by the Election Commission of India, any government body, or any political party. Do not use anything here in a real election.

## Goal

To design, in the open, an election system where **anyone can check that the count is correct, and any tampering or error is detectable and correctable**, while keeping every vote secret.

We aim for *evidence-based* elections, not "unhackable" ones. No system is perfect. The realistic target is that failures leave public evidence.

## Context

India's elections currently use EVMs with VVPAT paper trails, run by the Election Commission of India (ECI), which holds constitutional authority over elections. This project does not claim to replace that system. It explores what additional public verifiability could look like, and any real-world adoption would need the ECI, legal processes, and independent security review.

## Principles

1. **Non-partisan.** This is a technical project. Discussion of parties, candidates, or specific election results is out of scope.
2. **Threat model first.** Every design proposal must say which threats it addresses and which it does not.
3. **Prior art first.** We build on existing work (Helios, Belenios, ElectionGuard, Scantegrity, risk-limiting audits) before inventing new schemes.
4. **No overclaiming.** Security claims must be backed by a written argument or proof. Unreviewed cryptography is treated as broken.
5. **Paper-backed.** Software independence (an undetected software or hardware fault cannot change the outcome) is a design requirement.

## Scope

**In scope:** threat model, requirements, protocol design, public verification and audit methods, voter credential issuance, key management and tallying, usability, prototypes for research.

**Out of scope:** partisan advocacy, claims about past elections, and deployment in real elections.

## Open problems

These are the hard questions we need help with. Each has (or will have) a GitHub issue.

- [Cast-as-intended verification without enabling vote-selling or coercion](https://github.com/nakulBankura/projectGlassBox/issues/3)
- [Anonymous voter credentials without a central biometric database](https://github.com/nakulBankura/projectGlassBox/issues/4)
- [Long-term ballot privacy against future (including quantum) attackers](https://github.com/nakulBankura/projectGlassBox/issues/5)
- [Proof systems without a trusted setup](https://github.com/nakulBankura/projectGlassBox/issues/6)
- [Distributed key generation and tally availability](https://github.com/nakulBankura/projectGlassBox/issues/7)
- [Hardware trust: verifying the devices that are actually deployed](https://github.com/nakulBankura/projectGlassBox/issues/8)
- [Dispute resolution and remedies when something goes wrong](https://github.com/nakulBankura/projectGlassBox/issues/9)
- [Usability and accessibility across India's languages, literacy levels and scale](https://github.com/nakulBankura/projectGlassBox/issues/10)

## Repository layout

```
docs/threat-model.md     Start here
docs/requirements.md     Security and usability requirements
docs/decisions/          Short records of design decisions and why
research/                Prior art and reading list
specs/                   Protocol specifications
prototypes/              Research code (later)
```

## How to contribute

- Read `docs/threat-model.md` and challenge it. Missing threats are the most valuable contributions.
- Pick an open-problem issue and post your thoughts or a reading list.
- Add prior art to `research/` with a short summary.
- See `CONTRIBUTING.md` and `CODE_OF_CONDUCT.md`.
- Report security concerns privately as described in `SECURITY.md`.

## License

Code: Apache-2.0. Documentation: CC BY 4.0.

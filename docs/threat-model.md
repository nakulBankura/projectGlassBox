# Threat Model (draft v0)

This document is a starting point. Contributors are asked to challenge it, fill the gaps, and mark anything unresolved.

## 1. What we are protecting

- The **integrity** of the final tally
- The **secrecy** of each voter's choice
- The **eligibility** rule: only registered voters vote, once each
- The **availability** of voting and counting on election day

## 2. Security properties we want

| Property | Meaning |
|---|---|
| Ballot secrecy | No one can learn how an individual voted |
| Receipt-freeness | A voter cannot prove how they voted, even if they want to |
| Coercion resistance | A coercer cannot force or verify a voter's choice |
| Eligibility | Only eligible voters can cast a ballot |
| One voter, one vote | No double voting, no ballot stuffing |
| Cast-as-intended | The ballot records what the voter chose |
| Recorded-as-cast | The ballot is stored unchanged |
| Counted-as-recorded | The tally includes exactly the recorded ballots |
| Software independence | An undetected software or hardware fault cannot change the outcome |
| Long-term privacy | Ballots stay secret for decades, not just during the election |
| Availability | Attackers cannot block voting or the tally |

## 3. Adversaries

To be expanded. Initial list:

1. **Voter-level:** a coercer or vote-buyer (employer, local strongman, family member)
2. **Insider:** polling staff, election officials, or administrators
3. **Vendor:** hardware or software supply chain, including chip fabrication
4. **Network:** remote attackers, malware, denial of service
5. **State-level:** actors with large resources, including the ability to compel key-holders
6. **Future:** attackers who store data now and decrypt later (including quantum)

## 4. Trust assumptions

Every design must list what it trusts. Placeholder questions:

- Who generates and holds keys?
- Is any trusted setup ceremony required, and who runs it?
- Which devices must be honest, and how are they verified?
- What must the voter's own phone or device be trusted for?

## 5. Explicitly out of scope (for now)

- Voter registration roll accuracy and delimitation
- Campaign finance, media, and disinformation
- Physical violence at polling stations
- Legal and constitutional questions of adoption

## 6. Open questions

- How does a voter check cast-as-intended without gaining a transferable receipt?
- How is identity checked without creating a link between voter and ballot?
- What is the fallback if the electronic layer fails on election day?
- How are disputes and recounts handled?

## 7. Prior art to review

Helios, Belenios, ElectionGuard, Scantegrity II, Prêt à Voter, risk-limiting audits, the 2018 US National Academies report *Securing the Vote*, and ECI's existing EVM and VVPAT procedures.

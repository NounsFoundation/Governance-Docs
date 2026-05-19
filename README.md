# Nouns Foundation — Governance Documents

> **⚠️ DRAFT — NOT YET ADOPTED**
>
> Every document in this repository is a working draft. None has been adopted by the Nouns Foundation Board of Directors, and the Nouns Foundation itself has not yet been incorporated. The drafts are under review by Cahill Gordon & Reindel LLP (through its 501Foundry pro bono initiative), and are subject to revision before Board adoption, IRS application, and execution. Drafts are published openly so the Nouns DAO community can read, comment, and contribute to the governance design in the open.
>
> **Do not cite any document in this repository as a final or operative governance instrument of the Nouns Foundation.** Status will be updated here as documents are adopted.

---

## About the Nouns Foundation

The Nouns Foundation is a Delaware nonprofit nonstock corporation organized exclusively for charitable, educational, and other purposes within the meaning of Section 501(c)(3) of the Internal Revenue Code. Its mission is to advance the public good through charitable grants and related activities in four areas:

1. **Civic engagement and democratic participation** — supporting the study, development, and deployment of decentralized governance technologies and other initiatives that increase informed public participation in governance and strengthen civic institutions.
2. **Public goods, science, and technology** — advancing science and education through grants for open-source infrastructure, freely-licensed public technologies, and scientific research, including research conducted through decentralized or open-collaboration models.
3. **Arts and culture** — supporting the creation, presentation, and preservation of artistic and cultural works, including grants to individual artists and arts organizations.
4. **Community welfare** — supporting grassroots, community-based organizations and direct-impact initiatives that promote social welfare and serve communities and people in need.

The Foundation is intended to be classified as a public charity under Section 509(a)(1) or 509(a)(2) (final classification to be selected at the time of Form 1023 filing in consultation with legal counsel).

## Relationship to Nouns DAO

The Nouns Foundation operates **alongside** Nouns DAO — a Wyoming Decentralized Unincorporated Nonprofit Association (DUNA) — but is **structurally and legally independent** of it. The Foundation is its own legal entity with its own self-perpetuating Board, its own charitable purpose, and exclusive fiduciary authority over its own decisions.

Three structural facts define the relationship:

- **No appointment, removal, or veto authority.** Nouns DAO has no power to appoint, remove, replace, or veto any Director or officer of the Foundation, and no power to approve, veto, or compel any Grant or other action by the Foundation.
- **Recommendations are advisory only.** Nouns DAO may, through its governance process, submit non-binding *Recommendation Proposals* identifying charitable initiatives the Foundation may wish to consider. The Foundation's Board considers such recommendations in the exercise of its independent fiduciary discretion and is free to decline, modify, or grant to alternative recipients.
- **Two-layer privacy architecture.** Recommendations are submitted to the public Nouns DAO governance process at a high level; sensitive recipient information (PII, banking, KYC) is exchanged through a separate, private intake channel after recommendation passage. KYC is conducted using the Persona infrastructure operated for the benefit of the DUNA.

The operating framework between the two entities will be memorialized in a non-binding Memorandum of Understanding ([`agreements/DUNA-501c3-MOU.md`](agreements/DUNA-501c3-MOU.md)), to be executed following passage of an MOU Authorization Proposal by Nouns DAO.

## Repository Contents

```
.
├── Bylaws.md                                  Foundation Bylaws
├── policies/
│   ├── Conflict-of-Interest-Policy.md         COI framework + DUNA-Crossover Provisions
│   ├── Document-Retention-Policy.md           Records retention + on-chain records
│   ├── Whistleblower-Protection-Policy.md     Reporting channels + non-retaliation
│   ├── Compensation-Review-Process.md         §4958 rebuttable presumption procedure
│   ├── Grantmaking-Policy.md                  Grant approval framework
│   └── Director-Nomination-Policy.md          Nouns DAO nomination procedural framework
├── organizing-documents/
│   ├── Sole-Incorporator-Consent.md           DGCL §108 incorporator action
│   └── Initial-Board-Consent.md               DGCL §141(f) organizing board consent
├── agreements/
│   └── DUNA-501c3-MOU.md                      DUNA ↔ Foundation operating framework (form)
├── README.md                                  This file
└── LICENSE                                    CC0 1.0 Universal
```

### Reading order (suggested)

1. **[Bylaws](Bylaws.md)** — corporate constitution. Defines the Board, officers, Director Nomination Process, fiscal matters, and indemnification.
2. **[DUNA-501c3 MOU](agreements/DUNA-501c3-MOU.md)** — operating framework between Nouns DAO and the Foundation. Read this before the policies to understand the structural posture.
3. **[Conflict of Interest Policy](policies/Conflict-of-Interest-Policy.md)** — including the DUNA-Crossover Provisions in §6 that govern recusal and disclosure when Directors who are Nouns DAO participants consider Recommendation Proposals.
4. **[Grantmaking Policy](policies/Grantmaking-Policy.md)** and **[Director Nomination Policy](policies/Director-Nomination-Policy.md)** — the two policies that operationalize the Foundation's relationship with Nouns DAO recommendations.
5. **The remaining policies** ([Whistleblower](policies/Whistleblower-Protection-Policy.md), [Document Retention](policies/Document-Retention-Policy.md), [Compensation Review](policies/Compensation-Review-Process.md)) — standard §501(c)(3) governance instruments, with the structural specifics noted in each.
6. **Organizing documents** ([Incorporator Consent](organizing-documents/Sole-Incorporator-Consent.md), [Board Consent](organizing-documents/Initial-Board-Consent.md)) — adopt the Bylaws, elect officers, adopt the policies, and authorize the Form 1023 filing.

## Status and Roadmap

This is a pre-formation publication. The sequence is, roughly:

1. **Now — public drafting.** Documents in this repository are under review by Cahill / 501Foundry and open for community comment.
2. **Phase 2 — formation.** A successful Nouns DAO Formation Proposal authorizes incorporation. Certificate of Incorporation filed in Delaware. Sole Incorporator's Consent executed. Initial Board seated and Initial Board's Consent executed (which adopts Bylaws and policies, elects officers, authorizes Form 1023 filing).
3. **Phase 2 — exemption.** Form 1023 filed with the Internal Revenue Service. Determination letter recognizing §501(c)(3) status received (typical timeline: 3-12 months).
4. **Phase 3 — MOU execution.** A successful Nouns DAO MOU Authorization Proposal authorizes the DUNA Administrators to execute the DUNA-501c3 MOU. The MOU becomes effective on execution.
5. **Operations.** Grantmaking begins under the Grantmaking Policy. Document versions in this repository are updated to reflect the as-adopted form, with the DRAFT banner removed and a version-history table added.

Status updates will be reflected here as each step completes.

## Contributing and Comment

This repository is intentionally public and CC0-licensed. The Foundation welcomes substantive comment from the Nouns DAO community and from the broader public-interest legal and nonprofit-governance community.

- **Issues** — file an Issue on this repository to raise a question, flag an inconsistency, or propose a substantive change.
- **Pull requests** — pull requests are welcome for typographical corrections and clarity edits. Substantive governance changes will not be accepted via pull request before Board adoption; raise them as Issues instead.
- **Email** — Ian Wylie Hedrick (Wylie Advisory), governance partner for the formation, can be reached at `ian@wylieadvisory.com`.

This repository is also intended as a **resource for other DAOs** considering sister §501(c)(3) structures. The CC0 license permits free reuse and adaptation without attribution. If you fork this repository for that purpose, the Foundation would welcome (but does not require) a note indicating the use.

## License

All content in this repository is dedicated to the public domain under the [Creative Commons CC0 1.0 Universal](LICENSE) Public Domain Dedication. You may copy, modify, distribute, and use the documents, even for commercial purposes, all without asking permission and without attribution.

The CC0 dedication aligns with the Nouns DAO ethos of CC0 intellectual property and with the Foundation's mission to advance public goods.

## Acknowledgments

- **Cahill Gordon & Reindel LLP** (through 501Foundry) — pro bono incorporation and Form 1023 representation.
- **Wylie Advisory** — governance, policy, and operational structure.
- **The Nouns DAO community** — for the public-goods ethos that informs every line of this work.

# Structuring the Nouns Foundation

*How the research points to an independent 501(c)(3) — joined to Nouns DAO by non-binding recommendations — as the right design for a Nouns charitable arm.*

*A research report prepared by Wylie Advisory.*

---

## Executive summary

This report examines how Nouns DAO can best stand up a charitable arm — and why, across the available legal options and the real-world precedents, the analysis points to one design.

The Nouns Foundation, Inc. is a Delaware nonstock corporation formed to pursue federal tax-exempt status as a §501(c)(3) public charity. It is designed to give Nouns DAO a durable, tax-deductible, US-onshore vehicle for charitable grantmaking in four areas: civic engagement and democratic participation; public goods, science, and technology; arts and culture; and community welfare.

The defining structural choice is independence. The Foundation is a separate legal entity with its own self-perpetuating Board, its own charitable purpose, and exclusive fiduciary authority over its own decisions. Nouns DAO, a Wyoming Decentralized Unincorporated Nonprofit Association (DUNA), cannot appoint, remove, or veto any Director, and cannot approve, veto, or compel any grant. The DAO's role is to submit non-binding recommendations that the Board considers in the exercise of its independent fiduciary discretion.

That choice is not stylistic. It is the price of admission for tax-exempt charitable status. US tax law conditions both a charity's exemption and the deductibility of gifts to it on the charity retaining full control and ultimate discretion over its funds. A DAO that could direct the charity's grants or control its board would convert the charity into an instrument of the DAO and put the exemption at risk. Every major design decision in the governance package follows from that single constraint.

This document explains the design problem, the legal constraint that shapes it, the architecture chosen, the reasoning behind each major decision, and how the structure compares to the leading precedents — Big Green DAO, Endaoment, Gitcoin, and the offshore-foundation model used by ENS, Optimism, and Arbitrum. The short version: Big Green kept its DAO *inside* the charity; the offshore projects put their charity-equivalent *outside* the United States and gave up deductibility. The Nouns Foundation takes the harder, cleaner path — two independent US entities, a charity and a DUNA, joined only by non-binding recommendations.

## 1. The design problem

Nouns DAO wanted a charitable arm. The requirements were specific and partly in tension:

A charitable grantmaking vehicle that can make grants to US nonprofits, community organizations, and public-goods work, and have those grants treated as charitable under US law. Tax-deductibility for contributions into the vehicle, so the DAO's charitable capital — and any future donors — get the benefit US donors expect. Real US grantee relationships, since most intended recipients are US charities and community organizations that expect to receive funds from a recognized US charity. Legitimacy and permanence: an entity that reads as a real charity to grantees, regulators, auditors, and the public, not a marketing label on a DAO treasury.

At the same time, the DAO wanted to keep a meaningful voice in where the charitable dollars go, and the community wanted assurance that the vehicle would be accountable and could not be captured by any insider.

The tension is that the more control the DAO holds over the charity, the less the charity looks like an independent charity to the IRS, and the more its exemption and the deductibility of its funding are at risk. The entire structure is an answer to one question: how do we give the DAO a genuine voice without giving it the kind of control that breaks the charity?

## 2. The one rule that shapes everything: you can advise, but the charity decides

Almost every design choice below comes from a single rule in US tax law, so it is worth stating plainly.

When someone gives money to a charity, they get a tax deduction — but only if they actually give up control of the money. That is the catch. If you could still decide where the money goes after you have "donated" it, the law does not treat it as a real gift; it treats it as you spending your own money with a tax break attached. So the price of charitable tax treatment is that the charity — not the donor, and not anyone else — must hold the final say over how its funds are used. This is the *donor control* rule, and the IRS states it directly: a charity must keep full control of its funds and discretion over their use.

This one rule is why the law lets you *advise* a charity but never *control* it. You can suggest, recommend, and push hard for a cause. What you cannot do is tie the charity's hands — because the moment an outside party can force the charity's decisions, the charity stops being independent, and the tax benefits unravel for everyone.

Every established way to "have a say in charitable giving" is built around that line. Three that matter here:

- **Donor-advised funds (DAFs)** — the everyday version. You put money into a fund at a sponsoring charity and *recommend* where grants go. The charity legally owns the money and is never *required* to follow your recommendation, even though in practice it usually does. This is the model the Nouns structure most resembles: a body that recommends, a charity that decides.
- **Supporting organizations** — a charity that exists to support *another, already-existing* public charity (a university's endowment foundation is the classic example). To qualify, it has to be formally tied to the charity it supports — typically by letting that charity control its board. It buys a simpler tax status, but the price is exactly that control link.
- **Fiscal sponsorship** — a charity "hosts" a project that does not have its own tax status; the host owns the funds and keeps the right to claw them back if they are misused. This is how Big Green's DAO works — the project lives *inside* an existing charity rather than as its own entity.

The thread through all of them is the same: outsiders may advise; the charity's board must keep the final, legally binding decision. Any feature that lets an outside group *pick* the grants or *appoint* the board — a binding vote, a veto, the power to fire directors — crosses the line from advising to controlling, and puts both the tax exemption and the deductibility of every dollar flowing in at risk.

That is the entire reason Nouns DAO's recommendations are non-binding and the DAO holds no power to appoint, remove, or veto. These are not the Foundation holding the DAO at arm's length for its own sake. They are the load-bearing walls that let the charity be a charity at all.

*(For readers who want the underlying law: the donor-advised-fund rules are IRC §4966–4967, supporting organizations are §509(a)(3), and the "excess benefit" penalties that punish insiders who extract value from a charity are §4958. All are cited in the Sources.)*

## 3. The architecture chosen

The Foundation is built as a conventional, defensible US public charity, with a small number of carefully designed provisions that handle the novel DAO-recommendation flow.

**Entity.** A Delaware nonstock corporation, no members, pursuing §501(c)(3) recognition as a public charity (the §509(a)(1) or §509(a)(2) classification path is selected at the time of the Form 1023 filing). Delaware for its mature nonprofit corporate law and Court of Chancery *cy pres* mechanism; no members so that control rests solely with the Board and cannot be asserted by an outside body through membership rights.

**Board.** A self-perpetuating Board of five Directors, of whom at least three must be Independent Directors under the Form 990 four-prong definition. Staggered initial terms (3/2/2/1/1) so the Board cannot be turned over in a single year. The self-perpetuating, independent-majority board is the structural core of the charity's independence. See [`Bylaws.md`](Bylaws.md).

**The DAO relationship.** Nouns DAO may submit two kinds of non-binding proposals through its own governance process: Charitable Recommendation Proposals (identifying grant initiatives the Board may consider) and Director Nomination Proposals (identifying board candidates). In both cases the Board retains full discretion to decline, modify, or act otherwise, and a cap limits the share of seats that the nomination process can touch in any year. See the [Grantmaking Policy](policies/Grantmaking-Policy.md) and [Director Nomination Policy](policies/Director-Nomination-Policy.md).

**The MOU.** A short, explicitly non-binding Memorandum of Understanding memorializes how the two entities coordinate. It is authorized by a DAO proposal and signed by the DUNA Administrators, but it creates no enforceable obligations and hands neither side control over the other. See [`agreements/DUNA-501c3-MOU.md`](agreements/DUNA-501c3-MOU.md).

**Privacy and KYC.** A two-layer architecture: recommendations enter the public DAO process at a high level, while sensitive recipient information (PII, banking, KYC) flows through a separate private intake channel after a recommendation passes, leveraging the Persona KYC infrastructure operated for the DUNA.

**Brand.** Nouns artwork and identity are CC0 (public domain), so no brand license is needed between the entities, removing a category of affiliated-entity entanglement that ordinarily has to be papered.

## 4. Key design decisions and why they were made

### 4.1 Two independent entities, not a DAO inside the charity

The most consequential decision was to make the Foundation a *separate legal entity* from the DAO, rather than housing a "Nouns grants DAO" inside an existing charity as an internal program. The independent-entity path is harder: it forfeits the simplicity of a charity that simply owns the treasury and runs grant votes as its own internal process. But it produces a cleaner independence posture, keeps the DAO's governance and the charity's fiduciary decision-making in separate legal domains, and avoids any argument that the charity is merely the DAO's alter ego. The Foundation's board, not the DAO, is the legal grantor of record for every grant.

### 4.2 Public charity, not private foundation

Every §501(c)(3) is a private foundation by default unless it qualifies as a public charity under §509(a)(1)–(4). Public-charity status carries higher donor-deduction limits and avoids the Chapter 42 private-foundation excise regime (self-dealing under §4941, mandatory distributions under §4942, and the rest). The Foundation targets public-charity classification under §509(a)(1) or §509(a)(2), with the specific path selected at filing based on the anticipated funding and revenue mix.

The trade-off to manage is the **public support test**: a public charity must draw support from a sufficiently broad base, and a charity funded predominantly by a single source — here, the DAO — risks tipping into private-foundation classification. The design treats this as an ongoing monitoring obligation (flagged in the Grantmaking Policy and tracked annually by the auditor) and deliberately frames the DUNA as a non-routine funder, leaving room for genuine third-party fundraising. This is also why the MOU disclaims routine money flow from the DAO.

### 4.3 Why not a "supporting organization"

As Section 2 described, a supporting organization is a charity built to support *another, already-existing* public charity. On its face it looks like a tidy way to formally tie the Foundation to Nouns — but it does not fit, for a simple reason: **Nouns DAO is not a charity.** A supporting organization needs an existing public charity to support, and the DAO is a Wyoming DUNA, not a §501(c)(3). There is nothing for the Foundation to be a "supporting organization" *of* — the Foundation *is* the charity. And even if the fit were forced, qualifying would mean handing the supported entity control over the Foundation's board, which is the exact control link the whole design exists to avoid.

There is one honest trade-off worth naming. Supporting organizations are often used precisely to *escape* the public support test described in §4.2 — the requirement that a public charity draw on a broad funding base. Because the Foundation may lean heavily on DAO funding early on, that test is a real thing to manage. We chose to manage it directly — through monitoring and genuine third-party fundraising — rather than buy our way out of it by accepting a control relationship we would then have to explain away.

### 4.4 Staying clearly *not* a donor-advised fund

Section 2 introduced donor-advised funds — the "you recommend a grant, the charity decides" arrangement. Because the DAO recommends grants, there is a risk the IRS could try to treat the whole Foundation as one big donor-advised fund for the DAO. That label matters: it would trigger a separate set of taxes and restrictions and would blur the "independent charity" story the structure depends on. So the design deliberately keeps the Foundation from looking like one.

Three things do that work. The DAO is treated as one source of grant ideas among many, not the only pipeline. Every recommendation runs through the same review and diligence the Board applies to any grant idea, rather than a rubber-stamp lane. And the MOU states plainly that the Board may decline a recommendation, change it, fund a different recipient, or decline even to take it up — the cluster of "we are not obligated" statements that separates *recommending* a grant (fine) from *directing* one (not fine).

### 4.5 The non-binding director-nomination mechanism and the 40% cap

The DAO can identify board candidates through Director Nomination Proposals, but the mechanism is carefully bounded so that it informs rather than controls board composition. The bylaws make the character explicit: the recommendation is non-binding; the DAO has no appointment or removal power; the process is a procedural duty to *consider*, not a prerequisite to seating a director; and the Board reserves all authority. A cap limits the process to no more than 40% of seats in any year — comfortably below the 50% line that anchors the IRS independence analysis — so the DAO-informed path can never reach a controlling share of the Board. The vetting standard is substantive (modeled on the Wikimedia trustee review process) precisely so the consideration cannot be characterized as rubber-stamping, and the Board's content-neutrality rule means DAO-sourced candidates get no preference over Director-identified ones.

This is the centerpiece of the Form 990 defense: it lets the Foundation answer "No" to the Part VI questions about whether any outside person may elect or appoint members of the governing body, while still giving the community a real voice in succession. See the [Director Nomination Policy](policies/Director-Nomination-Policy.md).

### 4.6 The non-binding MOU

The MOU is deliberately thin — well under 1,500 words of operative text — and its single most important feature is that it is not a contract. Its non-binding character is stated in both the recitals and an operative section (belt-and-suspenders, because an instrument's binding character turns on the parties' expressed intent). It memorializes the recommendation flow; it does not create it. There is no consideration, no enforceability, and no remedies. A carve-out preserves the ability of the entities to enter separate, genuinely binding agreements on discrete operational matters without that bleeding back to suggest the MOU itself is binding.

### 4.7 How compensation stays clean

Like any nonprofit, the Foundation can pay the people who do real work — but it pays through a specific, defensible procedure rather than by handshake. US law gives charities a safe path here: if pay is (1) approved by people who have no personal stake in it, (2) checked against what comparable organizations pay for comparable work, and (3) written down at the time, the law *presumes* the pay is reasonable, and the burden flips to the IRS to prove otherwise. The Foundation builds that three-part check into its [Compensation Review Process](policies/Compensation-Review-Process.md) (lawyers call it the §4958 "rebuttable presumption" procedure). Initial officer pay is set at zero; the ability to pay later is preserved but gated behind that procedure.

Two supporting details. Paying a director a *reasonable* amount for serving on the board does not cost that director their "independent" status — what would break it is paying a director as staff or as a contractor. And basic separation-of-duties rules apply: the person who records what the board decided cannot also chair the meeting, and the person who sets up a grant cannot also be the one who signs the check. These are the ordinary financial controls that auditors, donors, and the IRS expect.

### 4.8 Two-layer privacy and KYC

Recommendations are public at a high level through DAO governance, but recipient PII, banking details, and KYC documentation move through a separate private intake channel after a recommendation passes, using the Persona infrastructure already operated for the DUNA. This keeps sensitive personal data out of the public on-chain record while still allowing the Foundation to conduct the diligence its grantmaking policy and §501(c)(3) status require.

## 5. How this compares to precedent models

No existing project does exactly what the Nouns Foundation does — pair an independent US public charity with a separate US DUNA via non-binding recommendations. But four reference points frame the choice.

### 5.1 Big Green DAO — the closest analog, and the key contrast

Big Green DAO, launched in November 2021 by Kimbal Musk's nonprofit Big Green, was billed as the first nonprofit-led philanthropic DAO. It runs participatory grantmaking to grassroots food and gardening organizations and is still operating (its public materials have since de-emphasized the "DAO/web3" framing in favor of "community-led grants").

The decisive fact: **Big Green DAO is not a separate legal entity.** It operates under the umbrella of Big Green's §501(c)(3) and is fiscally sponsored by it. The treasury is a conventional bank account owned by the Big Green charity, which "shoulders the administrative burden" and "ensures the tax-exempt status of donations." The DAO is, in legal substance, an internal participatory grant-selection process of an existing charity — closest to Model A fiscal sponsorship — and the charity's board retains legal control throughout. Big Green's own Form 990 shows full-board control of grantmaking with no separate grants committee, and no Schedule R or narrative treating the DAO as a separate organization.

Big Green is therefore strong precedent for one proposition — that a charity may use a community-voting process to exercise its own grantmaking discretion without losing its exemption — but it never had to solve the problem the Nouns Foundation solves, because its DAO was never a separate party to the charity. Nouns is doing the harder thing: keeping the DAO as a genuinely independent entity that recommends to, rather than operates within, the charity. That forfeits Big Green's "the charity just owns the treasury" simplicity in exchange for a cleaner separation of governance domains and a more defensible independence story.

### 5.2 Endaoment — advisory voting is already compatible with exemption

Endaoment is a California nonprofit public benefit corporation, federally tax-exempt as a §501(c)(3) community foundation (EIN 84-4661797), that operates on-chain donor-advised-fund infrastructure. Donors contribute crypto or other assets, receive a tax receipt, and *recommend* grants to US charities; Endaoment's "Community Funds" even let token-holders collectively vote on recipients. Throughout, the sponsoring charity retains ultimate discretion and is not bound to follow recommendations.

Endaoment is the cleanest proof that "a community votes on grants" and "the charity retains binding legal discretion" are a settled, operating, IRS-recognized combination — precisely because the votes are styled as non-binding advice to a charity that holds control. The difference is structural: Endaoment's recommenders are donors to DAFs *inside* the charity, whereas the Nouns Foundation's recommender is a *separate* DUNA. Nouns essentially lifts the DAF-style advisory relationship up to the entity level, with the DUNA in the donor-advisor role and the Foundation as the sponsoring-organization analog — while expressly disclaiming actual DAF status to stay outside §4966/§4967.

### 5.3 Gitcoin — the "skip the US charity" counterexample

Gitcoin funds open-source software and public goods, primarily through quadratic funding. Following a governance proposal, the Gitcoin DAO adopted a **Cayman Islands foundation company** as its real-world legal wrapper, not a US charity, and it does not offer US tax-deductibility for its grants.

That choice fits Gitcoin's facts: many of its grantees are individual developers and for-profit projects, and much of what it funds is not §501(c)(3)-eligible charitable activity, so a US charity would create private-benefit problems and offer little upside. The Nouns Foundation makes the opposite choice deliberately, because it *does* want charitable-class grantees and US-deductible contributions — which is exactly what forces the donor-control discipline that Gitcoin gets to skip.

### 5.4 The offshore foundation model — ENS, Optimism, Arbitrum (and Uniswap's DUNA)

The dominant "DAO legal wrapper" pattern is an ownerless offshore foundation — typically a Cayman, Swiss, or Panama foundation company. ENS, Optimism, and Arbitrum all use Cayman foundations to represent their DAOs. These vehicles provide token-holders limited liability and are tax-neutral and unconstrained by charitable-purpose rules — they can fund anything — but they give up US charitable tax-deductibility and are not bound by §501(c)(3) private-benefit, private-inurement, or §4958 rules.

Notably, the legal frontier is moving onshore: in 2025 Uniswap proposed adopting a **Wyoming DUNA** ("DUNI") for its governance layer — the same structure Nouns DAO already uses. That lets the Nouns architecture be positioned as something none of the offshore monoliths offer: a fully onshore, two-entity US design — a Wyoming DUNA for the DAO and a Delaware §501(c)(3) for the charity — rather than a single offshore foundation doing everything.

### 5.5 Comparison at a glance

| Model | Charity entity | Where the DAO sits | US tax-deductible? | Who controls grants |
|---|---|---|---|---|
| **Nouns Foundation** | DE nonstock §501(c)(3) public charity | Separate WY DUNA, recommends only | Yes | Independent Foundation Board |
| **Big Green DAO** | Existing US §501(c)(3) (Big Green) | Inside the charity (fiscally sponsored) | Yes | Charity board, via community vote process |
| **Endaoment** | CA §501(c)(3) community foundation | Donors/token-holders advise DAFs inside it | Yes | Sponsoring charity (advice non-binding) |
| **Gitcoin** | None (Cayman foundation company) | The foundation *is* the DAO wrapper | No | DAO / quadratic funding |
| **ENS / Optimism / Arbitrum** | None (Cayman foundation) | The foundation *is* the DAO wrapper | No | DAO governance |

## 6. Why this is the right trade

The Nouns Foundation is choosing constraint over flexibility, on purpose. An offshore foundation would let the DAO fund anything with no donor-control discipline — but it would forfeit US deductibility, charitable legitimacy, and clean relationships with US charitable grantees. Housing a grants DAO inside an existing charity (the Big Green path) would be simpler — but it would mean the charitable arm is not really the DAO's own institution and never achieves independent legal standing.

By standing up an independent US public charity and connecting it to the DAO only through non-binding recommendations, Nouns gets the things it actually wanted — deductibility, charitable legitimacy, US grantees, permanence, and a real community voice — and accepts the discipline that comes with them: the Board must hold ultimate discretion, the DAO cannot control the Board, and recommendations stay advisory. That discipline is not a constraint on the mission; it is what makes the mission legally durable, and it is what prevents any single actor — including any insider — from capturing the charity.

## 7. Open items and evolving law

A few matters remain under counsel review or depend on law that is still developing:

The §501(c)(3) **public charity classification path** (§509(a)(1) vs §509(a)(2)) is selected at the time of the Form 1023 filing based on the anticipated funding model, and the **public support test** will require ongoing monitoring given the DAO-weighted funding base. The **DAF regulations** proposed by Treasury in November 2023 (defining "donor-advisor," "advisory privileges," and "more than incidental benefit") are not yet final; if the structure were ever characterized as DAF-like, the final regulations would matter, which is one reason the MOU disclaims DAF status so directly. Several calibration parameters — the exact nomination-seat cap, the "material DAO participation" threshold in the conflicts policy, multisig configuration, and compensation comparability methodology for a small board stewarding a substantial treasury — are set at working values and are being confirmed with counsel. And the decision whether to **attach the MOU to the Form 1023** is open; Big Green's empirical filing posture suggests holding it back as a post-determination document may be cleaner.

None of these unsettle the core architecture. They are the normal calibration and watch-items of standing up a public charity, and each is being handled on the conservative side.

## Sources

**Donor control and exempt-organization fundamentals**

- IRS Exempt Organizations CPE — donor control doctrine: <https://www.irs.gov/pub/irs-tege/eotopico99.pdf>
- IRS Donor-Advised Fund Guide Sheet: <https://www.irs.gov/pub/irs-tege/donor_advised_explanation_073108.pdf>
- IRS EO CPE Text FY2003, "Public Charity or Private Foundation": <https://www.taxnotes.com/research/federal/irs-guidance/irs-cpe-textbooks/irs-eo-cpe-text-for-fiscal-2003-public-charity-or/zt6z>

**Donor-advised funds**

- IRC §4966 / §4967; Treasury proposed regulations on taxable distributions from donor-advised funds (Nov. 14, 2023): <https://www.federalregister.gov/documents/2023/11/14/2023-24982/taxes-on-taxable-distributions-from-donor-advised-funds-under-section-4966>
- DAF sponsor discretion / non-binding advice — National Philanthropic Trust, grantmaking rules: <https://www.nptrust.org/what-is-a-donor-advised-fund/grantmaking-rules/>

**Supporting organizations and public-charity classification**

- Adler & Colvin, "Public Charity Status Under §509(a)(3): The Supporting Organization": <https://www.adlercolvin.com/wp-content/uploads/2017/12/Public-Charity-Status-Under-Internal-Revenue-Code-Section-509a3-The-Supporting-Organization.pdf>
- IRS Publication 6016 (Type II supporting organizations): <https://www.irs.gov/pub/irs-pdf/p6016.pdf>
- §509(a)(1) vs §509(a)(2): <https://www.501c3.org/509a1-vs-509a2-nonprofit/>

**Fiscal sponsorship**

- Fiscal sponsorship models (variance power): <https://fiscalsponsorship.com/the-models-summary/>

**Big Green DAO**

- Big Green grantmaking: <https://biggreen.org/grantmaking/>
- Big Green DAO: <https://dao.biggreen.org/home>
- Caritas Law Group / Charity Lawyer Blog — nonprofit DAOs analysis: <https://charitylawyerblog.com/2023/01/02/blockchain-applications-in-the-nonprofit-sector-part-iii-decentralized-autonomous-organizations/>

**Endaoment**

- Endaoment legal / org registration (501(c)(3), EIN 84-4661797): <https://legal.endaoment.org/orgs>

**Gitcoin**

- Gitcoin governance proposal — "The Gitcoin Foundation: a Cayman Islands Foundation to represent the DAO IRL": <https://gov.gitcoin.co/t/proposal-the-gitcoin-foundation-a-proposal-to-represent-the-gitcoin-dao-irl-by-a-cayman-islands-foundation/9983>

**Offshore DAO foundations**

- ENS Foundation: <https://docs.ens.domains/v/governance/the-ens-foundation>
- Optimism Foundation FAQ: <https://community.optimism.io/welcome/faq/what-is-the-optimism-foundation>
- Mourant — "Cayman Islands foundation companies: the ideal vehicle for DAOs": <https://www.mourant.com/news-and-views/updates/updates-2024/cayman-islands-foundation-companies--the-ideal-vehicle-for-daos-and-crypto-trading.aspx>
- Uniswap "DUNI" Wyoming DUNA proposal: <https://vote.uniswapfoundation.org/proposals/90> · coverage: <https://decrypt.co/334355/uniswap-proposal-dao-legal-certainty-foundation-counsel>

---

*Descriptions of third-party organizations reflect public sources as of mid-2026. Evolving items — especially the proposed DAF regulations and any project's current filings — should be re-verified before external reliance.*

# DeltaCoin Economy and Economic Value

## Design overview

DeltaCoin is conceived as a network economy in which each coin is intended to
be a unit of exchange associated with a PDF containing the coin's
documentation. The documentation gives participants a shared description of
the unit and its underlying assets. Standardized market and network rules are
intended to make units easier to interpret and use across the economy. Terms
should be used consistently with their stated definitions so participants can
build on a shared meaning rather than an implied or shifting one.

This document describes the proposed design. It does not assert that the
network, market rules, or mechanisms described here have been implemented.

## Coin documentation

The content associated with a DeltaCoin is restricted to PDF documentation.
Each PDF should define the coin and describe the relevant assets, including
references to the assets' original documentation. Reproducing original
documentation requires appropriate permission or another legal basis. The PDF
is the documentary basis for understanding what a unit represents; the coin
should not be treated as a substitute for that documentation.

For the design to be useful in practice, the relationship between a coin and
its PDF, and the relationship between the PDF and the original asset
documentation, need to be clear to participants.

## Economy and participant contributions

Participants contribute to a chained economy by developing and supporting the
network and its units. The design identifies the following as potential
components:

- **Exchange:** DeltaCoin units serve as an applied medium of exchange under
  standardized market and network frameworks.
- **Engineering:** Participants support the system and may develop additional
  utility around existing coins.
- **Provenance records:** The ledger can record coin documentation and related
  intellectual-property claims or attribution.
- **Automated rules:** Smart contracts can carry out agreed transaction rules.
- **Trading and custody:** Network mechanisms may support trading, issuing, and
  transferring custody of assets. If an arrangement gives participants
  stock-like or other equity interests, it requires separate legal analysis.

These are design goals, not guarantees. A ledger entry alone does not create
intellectual-property rights, establish ownership, or protect a claim. A
smart contract does not by itself establish the parties' agreement or make an
arrangement legally enforceable.

## Economic value

In this design, a unit's value is the cumulative utility it represents across
the broader economy: its ability to assist participants and provide a
foundation for further development. This is a conceptual definition of value,
not a promise of market price, liquidity, or appreciation.

Participants may build on or refine an existing coin to create sub-coins. This
creates a tiered structure in which a sub-coin's pricing can be based on an
established on-chain DeltaCoin and its PDF documentation. The specific
information and specifications in the coin PDFs, including the references to
original asset documentation, are intended to inform pricing and trade ratios.
This does not establish a formula or objective market value: the relationship
between a parent coin and a sub-coin, and the rules for setting prices and
ratios, are not defined by this design description.

The design also intends for creators, suppliers, and users to contribute
useful, technically grounded content that supports the wider community.
Reliable sourcing, clear definitions, and verifiable specifications can help
discourage misinformation, but the design does not specify a validation or
incentive mechanism that guarantees accuracy. As a simple illustration of
definition-based meaning, the digit 1 remains one by definition even when
larger economic constructs are built on it; the analogy does not itself
establish a coin's utility or value.

## Scope of transfers

The intended economic model concerns the transfer of scarcity and value
represented by a unit, rather than a transfer of ownership or legal rights by
virtue of the coin alone. In particular, recording or transferring a coin
should not be interpreted by itself as transferring title to an underlying
asset, intellectual-property rights, shares, or custody. Any such rights or
arrangements must be defined separately in the applicable documentation and
handled under applicable agreements and law.

This design intent is not a legal classification. Calling a coin a utility,
currency, sub-coin, or non-ownership unit does not decide what rights it
actually conveys or which laws apply. Those questions depend on the offering,
the rights and expectations created, how the coin is used, and the facts of
the transaction.

## U.S. legal issue spotting

This section is a high-level issue-spotting summary, not legal advice or a
determination that a DeltaCoin is or is not subject to any particular law.
The design has not specified a jurisdiction below the federal level, the
participants' roles, the rights conveyed, or how the system will operate.

- **Securities and equity:** The Securities Act definition of a security
  includes stock and investment contracts. Under *SEC v. W.J. Howey Co.*, the
  analysis looks to the economic reality of the arrangement, including whether
  purchasers invest in a common enterprise expecting profits from others'
  efforts. Calling a token a coin or limiting the stated transfer to scarcity
  does not resolve that analysis. Any issuance or trading of stock, equity
  interests, or tokens sold with investment-like rights or expectations needs
  fact-specific securities-law review, including applicable registration or
  exemption requirements.
- **Bitcoin comparison:** The CFTC treated Bitcoin as a commodity under the
  Commodity Exchange Act in its 2015 Coinflip enforcement order concerning
  Bitcoin options. Separately, the IRS treats digital assets as property for
  U.S. federal tax purposes. These are context-specific treatments under
  different laws; neither establishes that Bitcoin is never part of a
  securities transaction, nor determines DeltaCoin's classification.
- **Exchange and money transmission:** Describing a coin as a medium of
  exchange does not by itself determine regulatory status. Depending on the
  activities and roles involved, administering, exchanging, or transmitting
  convertible virtual currency for others may raise federal Bank Secrecy Act
  and FinCEN obligations; state money-transmission requirements may also
  apply.
- **Copyright and documentation:** Copyright protects qualifying original
  expression, not facts or ideas as such. Putting a document or its hash on a
  ledger does not establish ownership or grant a license to reproduce the
  source material. Under federal copyright law, a transfer of copyright
  ownership generally requires a written instrument signed by the rights
  owner or authorized agent. Coin documentation should identify sources and
  permissions and state clearly whether it grants any license or other rights.
- **Custody and asset rights:** A token transfer or control of a wallet does
  not necessarily transfer legal title to, or custody rights over, an
  underlying asset. The legal effect depends on the asset, the agreements, and
  applicable law. If a coin represents securities or customer assets, separate
  custody and intermediary rules may be relevant.
- **Smart contracts:** Federal law generally does not deny an electronic
  record or signature legal effect solely because it is electronic. That does
  not make every on-chain transaction a valid or enforceable contract;
  agreement, authority, required disclosures, and other legal requirements
  still matter, and state law can affect the result.

### Sources

- [Securities Act definition of “security,” 15 U.S.C. § 77b](https://www.law.cornell.edu/uscode/text/15/77b)
- [*SEC v. W.J. Howey Co.*, 328 U.S. 293 (1946)](https://www.law.cornell.edu/supremecourt/text/328/293)
- [CFTC Coinflip order announcement (2015)](https://www.cftc.gov/PressRoom/PressReleases/7231-15)
- [IRS: Digital assets](https://www.irs.gov/filing/digital-assets)
- [FinCEN: Application of FinCEN's regulations to certain business models involving convertible virtual currencies (2019 guidance)](https://www.fincen.gov/system/files/2019-05/FinCEN%20Guidance%20CVC%20FINAL%20508.pdf)
- [Copyright subject matter, 17 U.S.C. § 102](https://www.law.cornell.edu/uscode/text/17/102)
- [Copyright ownership transfers, 17 U.S.C. § 204](https://www.law.cornell.edu/uscode/text/17/204)
- [Electronic Signatures in Global and National Commerce Act, 15 U.S.C. § 7001](https://www.law.cornell.edu/uscode/text/15/7001)

## Open design details

The design description does not specify the chain or token standard, how PDFs
are linked to and kept consistent with coins, how scarcity is defined or
verified, how sub-coin relationships and pricing work, or how asset custody
and equity-related arrangements are governed, which jurisdictions and
participant roles are in scope, how documentation is validated or incentives
are structured, or how regulatory obligations will be met. Those details
require explicit protocol, legal analysis, and documentation before the
economy can be evaluated as an operational system.

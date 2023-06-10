
**Title:** Data Trust DAO

**The need:** 

An organization that seeks to steward data in line with the preferences of those that generate it and/or those impacted by it,  by representing their interests around who can use this data and how it is used.

**The solution:** 

The organization creates a data trust, a legal structure that provides independent stewardship of data that involve “one party authorizing another to make decisions about data on their behalf, for the benefit of a wider group of stakeholders [where] the independent person, group or entity stewarding the data takes on a fiduciary duty” ([ODI, 2018](https://theodi.org/article/what-is-a-data-trust/)). This legal structure serves as a wrapper for a DAO that leverages both decentralized storage and decentralized governance solutions to carry out the aims of the data trust.

**Technologies used:**

- Host software (e.g. online platforms, browser extensions, mobile applications, camera applications) or hardware (e.g. IoT devices, sensors, cameras) where data is generated or captured
- Data de-identification methods (e.g. [k-anonymization](https://epic.org/wp-content/uploads/privacy/reidentification/Sweeney_Article.pdf), [I-diversity](https://personal.utdallas.edu/~muratk/courses/privacy08f_files/ldiversity.pdf), [t-closeness](https://www.cs.purdue.edu/homes/ninghui/papers/t_closeness_icde07.pdf), [pseudonymization](https://www.enisa.europa.eu/publications/pseudonymisation-techniques-and-best-practices/@@download/fullReport)) and tools (e.g. [ARX](https://arx.deidentifier.org/development/framework/), [Amnesia](https://amnesia.openaire.eu/), [Anonimatron](https://github.com/realrolfje/anonimatron))
- Content encryption methods (e.g. [AES](https://pycryptodome.readthedocs.io/en/latest/src/cipher/aes.html), [RSA](https://cryptography.io/en/latest/hazmat/primitives/asymmetric/rsa/), [ECC](https://pycryptodome.readthedocs.io/en/latest/src/public_key/ecc.html)) and software (e.g. [GnuPG,](https://gnupg.org/) [OpenSSL](https://www.openssl.org/))
- Decentralized storage marketplaces (e.g. [Filecoin](https://filecoin.io/), [Storj](https://www.storj.io/), [Sia](https://sia.tech/), [Arweave](https://www.arweave.org/))
- Decentralized data exchange platforms (e.g. [Streamr Marketplace](https://streamr.network/discover/marketplace/), [Ocean Protocol](https://oceanprotocol.com/)) or proprietary data marketplace
- Token standards for membership, governance, or utility tokens (e.g. ERC-20 for fungible tokens or ERC-721 for non-fungible tokens on Ethereum and EVM-compatible chains)
- Smart contracts for token issuance, governance, rewards distribution, staking and other relevant functionalities
- Decentralized access control protocols (e.g. [Lit Protocol](https://litprotocol.com/)) or proprietary token-gated dApps (e.g. online platforms, browser extensions, mobile applications)
- Tokenholder governance frameworks (e.g. [Compound Governor Bravo](https://github.com/compound-finance/compound-protocol/blob/master/contracts/Governance/GovernorBravoDelegate.sol), [OpenZeppelin Governor](https://docs.tally.xyz/user-guides/tally-contract-compatibility/openzeppelin-governor)), voting platforms (e.g. [Tally](https://www.tally.xyz/), [Snapshot](https://snapshot.org/)) and discussion forums (e.g. [Discourse](https://www.discourse.org/), [Commonwealth](https://commonwealth.im/)

Data is generated or captured through various host software or hardware. To ensure the privacy of the data providers, de-identification methods are employed to anonymize the data. Encryption methods are utilized to secure the data further. The anonymized and encrypted data is then stored using decentralized storage rental marketplaces. Access to this data is managed through decentralized data exchange platforms or proprietary data marketplaces, in accordance with the trust's governance rules. Token standards may be employed within the DAO for membership and governance purposes, supported by smart contracts. Decentralized access control protocols or proprietary token-gated applications are used to ensure secure access to data and resources within the data trust DAO. Tokenholder governance frameworks, voting platforms, and discussion forums are leveraged to enable decision-making and communication among the DAO's members, dependent on the level of member governance participation set out in the mandate of the trust.

**Stakeholders involved:**

- Trustees managing the data on the behalf of stakeholders as data stewards
- Individuals, organizations, institutions or platforms that generate or collect the data stewarded by the trust as data providers
- Researchers, organizations, businesses or other interested parties who access and use the data managed by the trust as data consumers
- Node operators in the storage marketplace as storage providers

**Example of where this pattern is used today:**

Data trusts are a legal structure in contexts that call for the secure protection and responsible stewardship of sensitive person-related data, such as in online platforms, healthcare, education and smart cities. DAOs are in the nascent stages of experimenting with how to apply this legal mechanism with decentralized protocols and distributed digital communities.

**Case study:**

[Superset](https://www.supersetdao.com/) is a data trust DAO that aims to better reward people for contributing data, inform investment decisions, and increase the accountability of the corporate arm of this ecosystem.  Superset takes the legal form of a [Guernsey trust](https://www.lexology.com/library/detail.aspx?g=9c301554-46f6-4770-ad1d-4011f3439b6f). Superset’s data owners or trustors are users of the investment app Delphia, which collects user spending data in exchange for providing investment advice. Superset is entrusted with the responsible use and management of this data, negotiating with and auditing Delphia on behalf of DAO members to ensure that the latter group gets a “fair share of the value created from their data.” Superset also allows for members to participate in collective decision-making on some issues via governance processes.

Read more here: [https://www.supersetdao.com](https://www.supersetdao.com/)

**Potential challenges:**

Trusts may become targets for hackers or cybercriminals, potentially resulting in data leaks or breaches.

The legal and operational costs of establishing and staffing a data trust structure may be prohibitive for some data owner communities and organizations.

Achieving consensus among stakeholders with varying objectives might slow down decision-making processes, and data trusts may face challenges in effectively representing the diverse interests of all stakeholders.

Data trusts are complex and not yet widely understood, and there are limited existing examples to draw from, making building and operating a trust challenging due to a lack of best practices.

**Practices for implementation:**

Define a clear mission and set of objectives for the Data Trust, ensuring that its purpose and goals align with the interests and expectations of data owners and consumers.

Establish a robust data governance framework, including policies, procedures, and guidelines for data access, sharing, privacy, security, and compliance, while addressing the rights and responsibilities of all stakeholders.

Develop accountability mechanisms and communication channels for transparency in all stages of decision-making processes, allowing data owners to understand how and why decisions are made, and fostering confidence in the data trust’s operations.

Establish a sustainable funding model to support the data trust's operations, considering diverse revenue streams such as grants, fees, donations, or partnerships.

Build relationships with other data trusts and data innovation organizations to share knowledge, experiences, and best practices.

**Other contexts where this pattern could be implemented:**

Data trust DAOs could also be used to steward AI training data, climate data and other datasets where responsible and efficient data sharing can advance scientific and technological development.

**Links:**

[https://medium.com/block-science/we-need-more-control-over-our-own-user-data-43f267a817f5](https://medium.com/block-science/we-need-more-control-over-our-own-user-data-43f267a817f5) [https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4009205](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4009205)

[https://theodi.org/article/what-is-a-data-trust/](https://theodi.org/article/what-is-a-data-trust/)

**Suggested tags:** Sensitive Data, Data Stewardship, Legal Wrapper, Fiduciary Duty, Governance

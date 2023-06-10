**Title:** Data Union DAO

**The need:** 

Stakeholders, or an organization representing them, wish to profit from the utilization by third parties of valuable data that they produce or crowdsource during their use of an application.

**The solution:** 

The stakeholders form or join a data union DAO, where member-generated data is “offered as a product on a marketplace for potential buyers [with] money from data sales is used to reward its members for providing valuable data.” ([Data Union DAO, 2023](https://docs.dataunions.org/getting-started/intro-to-data-unions)). In this way, individuals can directly benefit from the process of value extraction from the data that they produce.

**Technologies used:**

- Host software (e.g. online platforms, browser extensions, mobile applications, camera applications) or hardware (e.g. IoT devices, sensors, cameras) where data is generated or captured
- Decentralized storage marketplaces (e.g. [Filecoin](https://filecoin.io/), [Storj](https://www.storj.io/), [Sia](https://sia.tech/), [Arweave](https://www.arweave.org/))
- Decentralized data exchange platforms (e.g. [Streamr Marketplace](https://streamr.network/discover/marketplace/), [Ocean Protocol](https://oceanprotocol.com/))
- Decentralized real-time data streaming and pub-sub networks (e.g. [Streamr](https://streamr.network/), [IPFS pubsub](https://github.com/ipfs/js-ipfs/blob/master/docs/core-api/PUBSUB.md), [libp2p pubsub](https://docs.libp2p.io/concepts/pubsub/overview/), [Gossipsub](https://github.com/libp2p/specs/tree/master/pubsub/gossipsub))
- Token standards for membership, governance, or utility tokens (e.g. ERC-20 for fungible tokens or ERC-721 for non-fungible tokens on Ethereum and EVM-compatible chains)
- Smart contracts for token issuance, governance, rewards distribution, staking and other relevant functionalities
- Decentralized access control protocols (e.g. [Lit Protocol](https://litprotocol.com/)) or proprietary token-gated dApps (e.g. online platforms, browser extensions, mobile applications)
- Tokenholder governance frameworks (e.g. [Compound Governor Bravo](https://github.com/compound-finance/compound-protocol/blob/master/contracts/Governance/GovernorBravoDelegate.sol), [OpenZeppelin Governor](https://docs.tally.xyz/user-guides/tally-contract-compatibility/openzeppelin-governor)), voting platforms (e.g. [Tally](https://www.tally.xyz/), [Snapshot](https://snapshot.org/)) and discussion forums (e.g. [Discourse](https://www.discourse.org/), [Commonwealth](https://commonwealth.im/)

Data is generated or captured through host software, such as online platforms, browser extensions, mobile applications, or hardware, like IoT devices, sensors, and cameras. Decentralized real-time data streaming and pub-sub networks are used to transmit data between data providers and the data union DAO. The captured data is then stored on decentralized storage rental marketplaces. Decentralized data exchange platforms, either integrated or created by DAO, provide a marketplace for data buying and selling, enabling users to monetize their data. Token standards on blockchain networks represent membership, governance, or utility tokens for the data union DAO. Smart contracts handle token issuance, governance, rewards distribution, staking and other relevant functionalities. Decentralized access control protocols or proprietary token-gated dApps ensure secure access management for the data and services within the DAO. Tokenholder governance frameworks, along with voting platforms, enable decentralized decision-making within the data union DAO. Discussion forums facilitate communication and collaboration among members.

**Stakeholders involved:**

- Individuals or organizations that contribute data to the data union as data providers
- Third-party buyers who purchase the data from the union’s marketplace for various purposes, such as research or marketing as the data consumers
- Node operators in the storage marketplace as storage providers

**Examples of where this pattern is used today:**

Data union DAOs can be implemented to monetize user behavior data collected by online and mobile applications, enabling advertisers to make better-informed decisions while rewarding users for their data.

**Case study:**

Swash is a browser extension that lets you earn from your data as you surf the web. By joining Swash's Data Union, users contribute anonymized or pseudonymized data, which is then sold on marketplaces to interested buyers, such as researchers or marketers. Swash members are rewarded with SWASH tokens for their contributions.

Read more here: [https://swashapp.io/static/files/paper/whitepaper-v1-july-2021.pdf](https://swashapp.io/static/files/paper/whitepaper-v1-july-2021.pdf)

Data union DAOs can also be applied in the context of vehicle data analytics, which is a growing market segment as digital technologies are integrated into cars and used by drivers.

**Case study:**

DIMO is a data union that allows drivers to stream their vehicle data and be rewarded with DIMO tokens for their contributions. This vehicle data can then be sold to car manufacturers and insurance companies.

Read more here: https://docs.dimo.zone/docs/overview/intro

**Potential challenges:**

Ensuring user privacy may prove challenging, as data union DAOs need to implement robust data anonymization and encryption processes to protect users' information.

Navigating the complex legal landscape surrounding data protection and sharing, particularly in regions with strict data protection laws, may prove challenging for data union DAOs.

Tokens may be subject to volatility which could negatively impact participants' motivation and the long-term sustainability of the data service DAO.

Tokens may create legal and regulatory risks for the DAO and its members.

**Practices for implementation:**

Engage and educate members to ensure they are informed about the use of their data, the reward structure, and any fees associated with the data union.

Create and maintain a strong community by engaging with members and encouraging feedback, fostering trust and collaboration among participants.

Prioritize user privacy by implementing stringent data anonymization, encryption, and secure storage processes to protect users' information and ensure compliance with relevant data protection regulations.

**Other contexts where this pattern could be implemented:**

Health and fitness data, enabling users to monetize their personal health information collected by mobile and wearable devices while maintaining privacy and security.

Environmental and traffic data collected by IoT devices in smart city ecosystems, supporting urban planning initiatives, traffic management, and environmental monitoring efforts.

**Links:**

[https://docs.dataunions.org/getting-started/intro-to-data-unions](https://docs.dataunions.org/getting-started/intro-to-data-unions)

[https://docs.dataunions.org/resources/existing-data-unions](https://docs.dataunions.org/resources/existing-data-unions)

**Suggested tags:** Data monetization, DAOs

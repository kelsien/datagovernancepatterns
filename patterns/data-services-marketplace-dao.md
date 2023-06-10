**Title:** Data Services Marketplace DAO

**The need:** 

A group, organization, or institution seeks to share data with stakeholders and create a marketplace for the provision of services performed on or with the data (for example, Compute Over Data) ([Filecoin, 2023](https://rfs.fvm.dev/#01c77142f95145fbb6ddefb351f1bccc))

**The solution:** 

The organization creates a data service DAO with tokens that represent stake in the DAO and associated governance rights, and that can also be used to pay for data services.

**Technologies used:**

- Decentralized storage marketplaces (e.g. [Filecoin](https://filecoin.io/), [Storj](https://www.storj.io/), [Sia](https://sia.tech/), [Arweave](https://www.arweave.org/))
- Decentralized compute platforms (e.g [IPVM](https://github.com/ipvm-wg/spec), [Fluence](https://fluence.dev/docs/learn/overview), [Bacalhau](https://docs.bacalhau.org/))
- Decentralized bandwidth solutions (e.g. [Filswan](https://www.filswan.com/))
- Token standards for membership, governance, or utility tokens (e.g. ERC-20 for fungible tokens or ERC-721 for non-fungible tokens on Ethereum and EVM-compatible chains)
- Smart contracts for token issuance, governance, rewards distribution, staking, access control and other relevant functionalities
- dApps (e.g. online platforms, browser extensions, mobile applications) for use by DAO contributors
- Decentralized access control protocols (e.g. [Lit Protocol](https://litprotocol.com/)) or proprietary token-gated dApps (e.g. online platforms, browser extensions, mobile applications)
- Tokenholder governance frameworks (e.g. [Compound Governor Bravo](https://github.com/compound-finance/compound-protocol/blob/master/contracts/Governance/GovernorBravoDelegate.sol), [OpenZeppelin Governor](https://docs.tally.xyz/user-guides/tally-contract-compatibility/openzeppelin-governor)), voting platforms (e.g. [Tally](https://www.tally.xyz/), [Snapshot](https://snapshot.org/)) and discussion forums (e.g. [Discourse](https://www.discourse.org/), [Commonwealth](https://commonwealth.im/)
- DAO operations tooling (e.g. [Safe](https://safe.global/), [Discord](https://discord.com/), [Collab.Land](https://www.collab.land/), [Juicebox](https://juicebox.money/), [Utopia Labs](https://www.utopialabs.com/))

DAO members contribute datasets and models to the DAO via a dApp. This data is stored on decentralized storage rental marketplaces. Data services are made possible through the integration of existing protocols and platforms, such as decentralized compute and bandwidth networks, or by other means as established by the DAO and its technical infrastructure. Token standards are used on blockchain networks to represent membership, governance, and/or utility tokens, the latter being a mode of payment for services performed on or with the data managed by the DAO. Smart contracts handle token issuance, governance, rewards distribution, staking, access control, and other relevant functionalities. Decentralized access control protocols or proprietary token-gated dApps are used for secure access management to the data and services within the DAO. Tokenholder governance frameworks, along with voting platforms, enable decentralized decision-making within the data service DAO. Discussion forums facilitate communication and collaboration among members. DAO operations tooling is used to manage treasury management, communication, and resource allocation.

**Stakeholders involved:**

- Individuals and organizations contributing datasets and models to the DAO as data providers
- Other organizations and other interested individuals as data service consumers
- Individuals and organizations offering services to be performed with or on the data as data service providers
- Node operators in the storage marketplace as storage providers
- Node operators in decentralized compute and bandwidth platforms as resource providers
- Token holders who have the right to vote on decisions and proposals that impact the goals, strategy and policies of the data DAO as data governance participants

**Where this pattern is used today:**

Data service DAOs are particularly relevant in the artificial intelligence (AI) and data science contexts as a way to share training datasets and models and connect supply and demand for computing power.

**Case study:**

Lagrange DAO is a data service DAO that offers data sharing and analytics infrastructure (“Lagrange Spaces) for research collaboration and a decentralized computing power renting network that allows community members to rent out their computing power to researchers and users. The DAO uses a token-based incentive system that rewards contributions to the DAO. These tokens can be used to pay for data services, rent computing power or participate in DAO governance.

Read more here: [https://docs.lagrangedao.org/lagrange-dao/](https://docs.lagrangedao.org/lagrange-dao/)

https://github.com/filecoin-project/devgrants/issues/1138

Data DAOs are also a relevant pattern in collective efforts for data preservation, incentivizing participants to contribute to the protection and maintenance of any kind of data that the DAO deems important.

**Case study:**

GlacierDAO is working to solve the problem of source code preservation with a DAO that replicates Git repositories that contain code deemed to be of public interest. It will allow users to pool funds together in order to fund the replication of these repositories on the Filecoin network, while also rewarding users who show alignment with community values by giving them higher voting power on repository curation.

Read more here: [https://hackmd.io/@mJkqiMHdTGuZtNSkFvw_hg/rJqNZssvi](https://hackmd.io/@mJkqiMHdTGuZtNSkFvw_hg/rJqNZssvi)

**Potential challenges:**

Tokenholder governance in a data service DAO may be subject to manipulation or attacks by large holders.

Tokens may be subject to volatility which could negatively impact participants’ motivation and the long-term sustainability of the data service DAO.

Tokenization may create legal and regulatory risks for the DAO and its members.

The lack of central authority to verify and monitor data provided by contributors may lead to overall lower data quality.

Data service DAOs may face challenges in standardizing data from different sources and ensuring interoperability.

Data service DAOs may struggle to gain traction and generate necessary network effects to create effective data markets, especially in areas where other platforms and modes of data-sharing are already established.

**Practices for implementation:**

Creating a DAO constitution or charter to clearly define the mission of the data service DAO and its initial principles, policies and procedures regarding the data that it manages, as well as explicitly defining the scope of token holder governance

Establishing working groups or subDAOs dedicated to data stewardship to maintain data quality and interoperability.

Creating clear and detailed technical documentation to ensure that important knowledge of the data architecture and technical infrastructure is shared beyond the founding members of the DAO.

Establishing legal wrappers for the DAO and potential subDAOs may reduce legal liability on DAO members as individuals (please note that regulations are changing constantly. Please seek your own legal advice as this is not legal advice).

Maintaining a rigorous and cautious approach to tokenomic design that seeks to keep volatility to a minimum and preempts any perverse incentives that would be detrimental to the sustainability of the data service DAO.

Exploring more streamlined approaches to governance that reduce the time required to reach consensus and action a decision such as reducing the number of voting stages or establishing a delegation system that uses constrained delegation.

Pre-empting risks of governance manipulation or attacks in the design of the voting system. Explore both financial and non-financial incentives to bootstrap the data service DAO’s network, potentially prioritizing data supply over demand in initial stages of the DAOs roadmap

**Other contexts where this pattern could be implemented:**

Data service DAOs may be applicable in contexts where data democratization, secure collaboration, and decentralized decision-making are prioritized, such as sharing scientific data for research communities or crowd science initiatives, curating cultural or historical datasets, and facilitating access to geospatial information for urban planning or environmental conservation efforts.

**Links:**

[https://filecoin.io/blog/posts/fvm-imaginarium-bringing-datadaos-to-the-next-level-with-fvm/](https://filecoin.io/blog/posts/fvm-imaginarium-bringing-datadaos-to-the-next-level-with-fvm/)

[https://github.com/kangaroo-data-dao/](https://github.com/kangaroo-data-dao/)

[https://github.com/rk-rishikesh/DataDAO](https://github.com/rk-rishikesh/DataDAO)

**Suggested tags:** Data services, Data governance

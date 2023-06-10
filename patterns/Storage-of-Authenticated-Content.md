**Title:** Storage of Authenticated Content

**The need:** 

A group, organization or institution seeks to capture and store data in such a way that certain properties of that data can be verified, and other parties can confirm that the verification process has taken place, and can’t be tampered with.

**The solution:** 

Rather than simply trusting, or asking others to trust that certain claims about stored data are true, groups or organizations establish a decentralized data storage system that verifies data at the point of capture, as well as proving that the data has not been tampered with through cryptographic verification.

**Technologies used:**

- Host software (e.g. online platforms, browser extensions, mobile applications, camera applications) or hardware (e.g. IoT devices, sensors, cameras) where metadata about the data is generated or captured
- Decentralized storage marketplaces (e.g. [Filecoin](https://filecoin.io/), [Storj](https://www.storj.io/), [Sia](https://sia.tech/), [Arweave](https://www.arweave.org/))
- Clients and applications for interacting with decentralized storage rental marketplaces, including command line interfaces (e.g. [Lotus](https://lotus.filecoin.io/lotus/get-started/what-is-lotus/) and [Venus](https://docs.filecoin.io/nodes/implementations/venus/) for Filecoin, [Uplink CLI](https://www.storj.io/integrations/uplink-cli) for Storj, [sia daemon](https://github.com/SiaFoundation/siad) for Sia) and graphical user interfaces (e.g. [Chainsafe Files](https://files.chainsafe.io/), [web3.storage](https://web3.storage/), [Estuary](https://estuary.tech/) and [Lighthouse](https://www.lighthouse.storage/) for Filecoin, [Satellite Web Interface](https://github.com/storj/storj/wiki/Satellite-GUI) for Storj, [Sia-UI](https://github.com/NebulousLabs/Sia-UI) for Sia)
- Cloud storage rental marketplaces nodes (e.g. [IPFS nodes](https://docs.ipfs.tech/concepts/nodes/#preload), [Filecoin nodes](https://spec.filecoin.io/systems/filecoin_nodes/), [Storj nodes](https://docs.storj.io/node), [Sia hosts](https://docs.sia.tech/hosting/about-hosting-on-sia))
- [IPFS nodes](https://docs.ipfs.tech/concepts/nodes/#preload)
- [Third-party remote pinning services](https://docs.ipfs.tech/how-to/work-with-pinning-services/) (e.g. [Pinata](https://www.pinata.cloud/), [Infura](https://docs.infura.io/infura/networks/ipfs/how-to/manage-files), [Crust](https://wiki.crust.network/docs/en/buildIPFSW3AuthPin), [Filebase](https://filebase.com/)) or [Filecoin-backed remote pinning services](https://filecoin.io/blog/posts/decentralized-storage-estuary-web3.storage-and-nft.storage/) (e.g. [nft.storage](https://nft.storage/), [web3.storage](https://web3.storage/), [Estuary](https://estuary.tech/))
- Blockchain/s (e.g. [Ethereum](https://ethereum.org/en/), [Polygon](https://polygon.technology/), [Hyperledger Fabric](https://www.hyperledger.org/use/fabric))
- Decentralized ordering, time-stamping and logging to decentralized protocols (e.g. [Ceramic](https://ceramic.network/), [Hedera Consensus Service](https://hedera.com/consensus-service))
- Decentralized graph data syncing to blockchains (e.g. [Gun Protocol](https://gun.eco/docs/))

Data is captured from a hardware device, where a set of assertions about the data are created at the moment of capture based on input from sensors in the device. These assertions are stored as metadata. If using Filecoin, files containing the data and metadata are imported using the client or application, transformed into content-addressable representations, CIDs are created and available storage providers are found. Storage deals based on the user’s requirements regarding the amount of data to be stored, storage duration and pricing are proposed to Filecoin storage providers using the client or application. The data associated with the CIDs are stored on the Filecoin network by storage providers. The data associated with the CIDs may also be pinned by user-run IPFS nodes or those engaged via remote pinning services for ongoing data availability, e.g. for the purposes of displaying on a website. Interactions with the data are logged to one or more blockchains using decentralized time-stamping and ordering solutions, so that any modifications to the original data will be transparently documented.

**Stakeholders involved:**

- Organizations or institutions as data providers and potentially hot storage providers
- Node operators in storage rental marketplaces as cold storage providers
- Remote pinning services as hot storage providers
- Audiences that the user wishes to share their data with as data consumers

**Example of where this pattern is used today:**

In times of misinformation and deep fakes, decentralized data storage that incorporates verification, tamper-proofing and transparency is useful in contexts of photojournalism, as well as in judicial settings such as in the documentation of war crimes.

**Case study:**

[Starling Lab](https://www.starlinglab.org/), [Reuters](https://www.reuters.com/) and blockchain data integrity startup [Numbers Protocol](https://www.numbersprotocol.io/) collaborated on the photojournalism project 78 Days, where they used Filecoin, Hyperledger Fabric, Hedera Consensus Service and IPFS, together with standards and technology developed by the Content Authenticity Initiative, to ensure 78 consecutive days of photographs produced by Reuters photojournalists were created with cryptographically secure metadata.

Read more here: [https://filecoin.io/blog/posts/tracking-78-days-of-the-us-presidential-election-on-filecoin/](https://filecoin.io/blog/posts/tracking-78-days-of-the-us-presidential-election-on-filecoin/)

**Potential challenges:**

The complexity and experimental nature of decentralized data verification and storage methodologies may result in a slower adoption rate.

Stakeholders take time to understand, trust, and integrate the technology into their workflows. Institutions, such as courts, may require further validation or standardization.

Some other challenges are documented [here](https://www.starlinglab.org/challenges/).

**Practices for implementation:**

Collaborate closely with hardware and software vendors to integrate data capture and verification functionalities directly into the devices and applications used for generating or collecting data.

Actively engage with and adopt existing content authentication and verification standards, such as the [Content Authenticity Initiative (CAI)](https://contentauthenticity.org/).

Engage with and educate data consumers, such as courts or the general public, about the verification process and its benefits.

**Other contexts where this pattern could be implemented:**

Scientific research, where maintaining data integrity and transparency is essential for the reproducibility and credibility of results.

IoT technologies, where ensuring data integrity and transparency is crucial to maintain trust and accuracy in the large amounts of information generated by interconnected devices and sensors. Supply chain management, where tracking and verifying product sources and quality is crucial for consumer trust and ethical business practices.

**Links:**

[https://www.starlinglab.org/image-authentication/](https://www.starlinglab.org/image-authentication/)

**Suggested tags:** Verification, Evidence, Institutions, Hardware


**Title:** Storage with Encryption and Private Storage Network

**The need:** 

An individual, group, organization or institution seeks to store data in a manner that is highly secure and private.

**The solution:** 

The group of people or organization encrypts the data, and uses decentralized data storage solutions where data is stored only by trusted storage providers and not publicly accessible except by trusted parties.

**Technologies used:**

- Content encryption methods (e.g. [AES](https://pycryptodome.readthedocs.io/en/latest/src/cipher/aes.html), [RSA](https://cryptography.io/en/latest/hazmat/primitives/asymmetric/rsa/), [ECC](https://pycryptodome.readthedocs.io/en/latest/src/public_key/ecc.html)) and software (e.g. [GnuPG,](https://gnupg.org/) [OpenSSL](https://www.openssl.org/))
- [IPFS private network](https://github.com/ipfs/kubo/blob/release-v0.9.0/docs/experimental-features.md#private-networks)
- Decentralized access control protocols (e.g. [Lit Protocol](https://litprotocol.com/)) or proprietary token-gated dApps (e.g. online platforms, browser extensions, mobile applications)
- Blockchains (e.g. [Ethereum](https://ethereum.org/en/), [Polygon](https://polygon.technology/), [Hyperledger Fabric](https://www.hyperledger.org/use/fabric))
- Decentralized ordering, time-stamping and logging to blockchains (e.g. [Ceramic](https://ceramic.network/), [Hedera Consensus Service](https://hedera.com/consensus-service))
- Optional additional privacy layers (e.g. [Tor](https://docs.ipfs.tech/how-to/privacy-best-practices/) Onion Router)

Data is encrypted using a method that meets the organization or group’s security requirements. The encrypted data is then transformed into a content-addressable representation with IPFS using CIDs. Blocks of the CIDs are saved on trusted nodes in an IPFS private network, which pin the CIDs to ensure data availability. In a private network, IPFS can only connect with other peers that have a shared secret key. Decentralized access control protocols may also be used to ensure that only trusted third parties can access the data. Decentralized ordering and time-stamping solutions can be used to log data-related events transparently and immutably to one or more blockchains.

**Stakeholders involved:**

- Individuals
- Organizations as both data providers and storage providers
- Trusted third parties that the organization wishes to share their data with as data consumers

**Example of where this pattern is used today:**

Encryption and private storage networks are useful in enterprise settings where sensitive and commercially significant data is exchanged among multiple parties.

**Case study:**

Morpheus.Network, a supply chain software-as-a-service (SaaS) platform, stores encrypted data and documents on a private network of IPFS nodes and event logging on the Ethereum blockchain, to ensure that shippers, authorities, and recipients can consistently retrieve shipment data, and to be assured that documents used in shipping transactions are verified and tamper-proof.

Read more here: [https://docs.ipfs.tech/case-studies/morpheus/#the-story](https://docs.ipfs.tech/case-studies/morpheus/#the-story)

**Implementation Practices:**

Establish a clear process for onboarding and vetting new storage providers in the IPFS private network, as well as for monitoring their performance and compliance with network requirements.

Regularly engage with data owners and consumers to gather feedback on their experiences with the encrypted storage and private storage network, addressing any concerns and continuously improving the system.

Stay informed about emerging security threats and best practices in encryption and data storage, regularly updating the system's security measures to maintain the highest level of protection.

Ensure that your encrypted storage and private storage network solution remains compliant across different jurisdictions.

**Potential challenges:**

Because IPFS private networks are designed to only connect a limited set of nodes, it inherently does not benefit from the scale, geographical resilience and faster retrieval times of the public IPFS network.

Latency and performance issues may arise from encryption and decryption processes, especially when dealing with large volumes of data or high levels of data access.

Advances in cryptography and computing power may render some encryption methods less secure over time, limiting data security [guarantees](https://docs.ipfs.tech/how-to/privacy-best-practices/).

Varying data privacy and security requirements across different jurisdictions may pose challenges for a globally compliant private network and encryption solution.

**Other contexts where this pattern could be implemented:**

Healthcare, where sensitive patient data must be shared among healthcare providers.

Financial services, where transaction data and user information must be kept secure.

Research institutions, where confidential research data needs to be securely shared among collaborators.

**Links:**

[https://docs.ipfs.tech/case-studies/morpheus/#case-study-morpheus-network](https://docs.ipfs.tech/case-studies/morpheus/#case-study-morpheus-network)

https://medium.com/pinata/dedicated-ipfs-networks-c692d53f938d

[https://blog.ceramic.network/how-to-store-signed-and-encrypted-data-on-ipfs/](https://blog.ceramic.network/how-to-store-signed-and-encrypted-data-on-ipfs/)

[https://github.com/ipfs/kubo/blob/release-v0.9.0/docs/experimental-features.md#private-networks](https://github.com/ipfs/kubo/blob/release-v0.9.0/docs/experimental-features.md#private-networks)

[https://docs.ipfs.tech/how-to/privacy-best-practices/](https://docs.ipfs.tech/how-to/privacy-best-practices/)

[https://docs.ipfs.tech/concepts/privacy-and-encryption/](https://docs.ipfs.tech/concepts/privacy-and-encryption/)

[https://discuss.ipfs.tech/t/encryption-private-data-and-private-swarms-with-ipfs/15363](https://discuss.ipfs.tech/t/encryption-private-data-and-private-swarms-with-ipfs/15363)

**Suggested tags:** Sensitive Data, Encryption, Privacy, Verification

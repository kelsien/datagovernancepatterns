**Title:** Encrypted content on public IPFS network

**The need:** 

An individual, group, organization or institution seeks to distribute encrypted data publicly

**The solution:** 

The individual or organization encrypts the data, and uses decentralized data storage solutions where data is stored only by trusted storage providers and not publicly accessible except by trusted parties.

**Technologies used:**

- Content encryption methods (e.g. [AES](https://pycryptodome.readthedocs.io/en/latest/src/cipher/aes.html), [RSA](https://cryptography.io/en/latest/hazmat/primitives/asymmetric/rsa/), [ECC](https://pycryptodome.readthedocs.io/en/latest/src/public_key/ecc.html)) and software (e.g. [GnuPG,](https://gnupg.org/) [OpenSSL](https://www.openssl.org/))
- [IPFS network](https://docs.ipfs.tech/)
- [IPFS nodes](https://docs.ipfs.tech/concepts/nodes/#preload)
- [Third-party remote pinning services](https://docs.ipfs.tech/how-to/work-with-pinning-services/) (e.g. [Pinata](https://www.pinata.cloud/), [Infura](https://docs.infura.io/infura/networks/ipfs/how-to/manage-files), [Crust](https://wiki.crust.network/docs/en/buildIPFSW3AuthPin), [Filebase](https://filebase.com/)) or [Filecoin-backed remote pinning services](https://filecoin.io/blog/posts/decentralized-storage-estuary-web3.storage-and-nft.storage/) (e.g. [nft.storage](https://nft.storage/), [web3.storage](https://web3.storage/), [Estuary](https://estuary.tech/))

Data is encrypted using a method that meets the organization’s security requirements. The encrypted data is then transformed into a content-addressable representation with IPFS using CIDs. Blocks of the CIDs are saved on IPFS nodes controlled by the organization or trusted third parties, and/or by remote pinning services.

**Stakeholders involved:**

- Organizations as data providers and storage providers
- Audiences that the organization wishes to share their data with as data consumers

**Example of where this pattern is used today:**

This pattern can be used when working with content that is considered a public good, that may be censored in some jurisdictions, but people would like to ensure the information is publicly replicated (to all people, or to a specific subset of a community or member group).

**Case study:**

Matters News is a web platform for crowd-sourced news in Chinese native language. People can create, search, and follow articles, tags and authors. The purpose of Matters News is “a better way of distributing content”. The platform allows for creators to monetize their content without relying on advertising by offering subscription models in both FIAT and cryptocurrency. Adoption has grown rapidly from its inception in 2018 to over 80,000 content creators and 6 million monthly users across Hong Kong, Taiwan, and China, as well as Oceania, the US and Europe. The Matters News website is built on IPFS so that everyday users can create and access news without having to worry about being censored. Matters News requires a geographically distributed content back-up solution to continue to host the platform if users can’t access it, the platform is down, or the company ceases to exist. A close competitor in choosing a content solution was Dat protocol (now Hypercore protocol) but IPFS was chosen for faster content distribution. When authors upload news content onto the platform, it is automatically content addressed to create an IPFS hash of the data, which is then stored in the metadata of that article. It then requires additional steps for encryption as IPFS network is public and everything is transparent during transportation. While public content on Matters News is publicly visible, the team adds a layer of encryption to exclusive content on the platform. Public key distribution is a challenge to allow the right users to decrypt this, which they have addressed with “symmetric” key encryption, meaning keys are distributed in subscriber channels, and the team must rely on users not to share these publicly.

Read more here: [](https://docs.ipfs.tech/case-studies/morpheus/#the-story) [https://ecosystem.ipfs.tech/project/matters-news/](https://ecosystem.ipfs.tech/project/matters-news/) ; [https://community.interledger.org/matters/web-monetization-on-ipfs-matters-2e93](https://community.interledger.org/matters/web-monetization-on-ipfs-matters-2e93)

**Potential challenges:**

Advances in cryptography and computing power may render some encryption methods less secure over time. As data is stored publicly on IPFS, it can be easily accessed and decrypted in this scenario, whereas while encrypted data stored on a private IPFS network may also be in theory decryptable in the future, it remains inaccessible to parties who do not meet access requirements.

Latency and performance issues may arise from encryption and decryption processes, especially when dealing with large volumes of data or high levels of data access.

Varying data privacy and security requirements across different jurisdictions may pose challenges for a globally compliant private network and encryption solution.

**Practices for implementation:**

Regularly engage with data owners and consumers to gather feedback on their experiences with the encrypted solutions, addressing any concerns and continuously improving the system.

Stay informed about emerging security threats and best practices in encryption, regularly updating the system's security measures to maintain the highest level of protection.

Ensure that your encrypted storage solution remains compliant across different jurisdictions.

See: [https://docs.ipfs.tech/how-to/privacy-best-practices/](https://docs.ipfs.tech/how-to/privacy-best-practices/)

**Other contexts where this pattern could be implemented:**

For information that may be culturally or politically sensitive, but people want to content address and replicate across and IPFS network, or share to a specific member group or community but can do so over a public network.

**Links:**

[https://blog.ceramic.network/how-to-store-signed-and-encrypted-data-on-ipfs/](https://blog.ceramic.network/how-to-store-signed-and-encrypted-data-on-ipfs/)

[https://docs.ipfs.tech/how-to/privacy-best-practices/](https://docs.ipfs.tech/how-to/privacy-best-practices/)

[https://docs.ipfs.tech/concepts/privacy-and-encryption/](https://docs.ipfs.tech/concepts/privacy-and-encryption/)

**Suggested tags:** Sensitive Data, Encryption, Public

**Title:** Individual-storage

**The need:**

Individuals seek to persistently store data and ensure it is retrievable by others over a long-term period.

**The solution:**

Rather than relying on centralized data storage solutions, users develop a custom solution combining decentralized data storage protocols and services that meet their individual needs for persistence and data availability.

**Technologies used:**

- [IPFS network](https://docs.ipfs.tech/)
- [IPFS nodes](https://docs.ipfs.tech/concepts/nodes/#preload)
- [IPFS Cluster](https://docs.ipfs.tech/install/server-infrastructure/)
- [Third-party remote pinning services](https://docs.ipfs.tech/how-to/work-with-pinning-services/) (e.g. [Pinata](https://www.pinata.cloud/), [Infura](https://docs.infura.io/infura/networks/ipfs/how-to/manage-files), [Crust](https://wiki.crust.network/docs/en/buildIPFSW3AuthPin), [Filebase](https://filebase.com/)) or [Filecoin-backed remote pinning services](https://filecoin.io/blog/posts/decentralized-storage-estuary-web3.storage-and-nft.storage/) (e.g. [nft.storage](https://nft.storage/), [web3.storage](https://web3.storage/), [Estuary](https://estuary.tech/))
- Decentralized long-term storage networks (i.e. [Arweave](https://www.arweave.org/))

Files are transformed into a content-addressable representation with IPFS using CIDs. Blocks of the CIDs are saved on an IPFS node or nodes. These could be a user’s personal node or set of nodes as part of their IPFS Cluster, the set of nodes managed by a remote pinning service or a combined Filecoin and IPFS solution. CIDs are pinned by these nodes and made publicly discoverable on the IPFS network. Users may opt to save and pin CIDs to multiple nodes for improved redundancy and resilience, e.g. pinning to their personal node as well as using a remote pinning service. Alternatively, users may opt to use [Arweave](https://www.arweave.org/) alongside IPFS and its associated solutions, uploading their files to the Arweave network for a one-time fee.

**Stakeholders involved:**

- Users as both data providers and storage providers, as well as potentially data consumers
- Remote pinning services teams as additional storage providers (including Filecoin storage providers if using Filecoin-backed remote pinning services)
- Audiences that the user wishes to share their data with as data consumers

**Example of where this pattern is used today:**

NFTs hold associated metadata that provides information about the digital asset, such as the creator, description, and the actual digital file (e.g., artwork, music, or collectible). Storing NFT data stored only on centralized servers poses a risk to the resilience of NFTs. If the server goes down or the service provider ceases operations, the NFT's metadata may become irretrievable and no longer usable or valuable. To avoid this, NFT artists and collectors may use decentralized storage solutions to protect the cultural and financial value of NFTs.

**Case study:**

Visual artist and collector OficiniasTK used IPFS, Raspberry Pi and Pinata to create a resilient self-storage solution for their NFTs.

Read more here: [https://medium.com/pinata/how-to-build-a-portable-nft-display-cae5dc12727e](https://medium.com/pinata/how-to-build-a-portable-nft-display-cae5dc12727e)

Websites also benefit from decentralized storage for hosting, as it enhances reliability, reduces the risk of single points of failure, and improves resistance to censorship. By distributing website data across multiple nodes in a decentralized network, content becomes more resilient to server outages or targeted attacks.

**Case study:**

ShapeShiftDAO decentralized their frontend by hosting it on IPFS.

Read more here: [https://medium.com/@ShapeShift.com/ipfs-a-journey-to-complete-decentralization-f4dfd1be552a](https://medium.com/@ShapeShift.com/ipfs-a-journey-to-complete-decentralization-f4dfd1be552a)

**Potential challenges:**

- The cost of decentralized self-storage solutions may be more difficult to ascertain then with using a centralized service provider. Individuals need to evaluate the trade-offs between decentralization and greater control over their data infrastructure, and centralization with less control but potentially lower costs in some cases.
- Decentralized self-storage solutions may have slower data retrieval times compared to centralized solutions, which could affect the overall user experience.
- Implementing decentralized self-storage solutions can be more complex compared to centralized solutions, which may pose a challenge for users with limited technical expertise.

**Practices for implementation:**

- Combine multiple storage solutions or services to increase data availability and resilience against potential failures.
- Regularly evaluate and update the chosen storage solutions and services to ensure they remain reliable, secure, and aligned with the user's needs and expectations.
- Educate oneself on the various decentralized data storage protocols, services, and best practices, and actively engage with online communities, forums, and resources to stay informed and troubleshoot potential issues.
- Schedule and perform regular maintenance of personal nodes and storage infrastructure, including software updates, security patches, and hardware health checks.

**Other contexts where this pattern could be implemented:**

Individuals can adapt self-storage patterns for a variety of personal use cases beyond NFTs, from academics and creatives seeking to preserve and make available their body of work for posterity, to families seeking a way to store important genealogical documents and records for future generations.

**Links:**

[https://docs.ipfs.tech/how-to/best-practices-for-nft-data/](https://docs.ipfs.tech/how-to/best-practices-for-nft-data/)

[https://docs.ipfs.tech/how-to/work-with-pinning-services/](https://docs.ipfs.tech/how-to/work-with-pinning-services/)

[https://docs.ipfs.tech/install/server-infrastructure/](https://docs.ipfs.tech/install/server-infrastructure/)

[https://kelsienabben.substack.com/p/not-your-storage-architecture-not](https://kelsienabben.substack.com/p/not-your-storage-architecture-not) [https://thedefiant.io/do-you-really-own-your-nft-chances-are-you-dont](https://thedefiant.io/do-you-really-own-your-nft-chances-are-you-dont)

**Suggested tags:** Persistence, Public Data, Cultural Data, Individuals

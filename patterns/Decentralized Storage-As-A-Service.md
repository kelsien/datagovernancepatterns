**Title:** Decentralized Storage-As-A-Service

**The need:** 

An individual, group, organization or institution seeks to persistently store larger volumes of data over a long-term period, and may additionally seek to ensure this data is retrievable by the public.

**The solution:**

Rather than relying on centralized data storage solutions, or on self-run IPFS nodes and remote pinning services, a person or organization can engage storage providers on a decentralized storage rental marketplace, where storage and retrieval agreements are incentivized and enforced through cryptocurrency token rewards and cryptographic proofs respectively.

**Technologies used:**

- Decentralized storage marketplaces (e.g. [Filecoin](https://filecoin.io/), [Storj](https://www.storj.io/), [Sia](https://sia.tech/), [Arweave](https://www.arweave.org/))
- Clients and applications for interacting with decentralized storage rental marketplaces, including command line interfaces (e.g. [Lotus](https://lotus.filecoin.io/lotus/get-started/what-is-lotus/) and [Venus](https://docs.filecoin.io/nodes/implementations/venus/) for Filecoin, [Uplink CLI](https://www.storj.io/integrations/uplink-cli) and [Filezilla](https://www.storj.io/integrations/filezilla) for Storj, [sia daemon](https://github.com/SiaFoundation/siad) for Sia) and graphical user interfaces (e.g. [Chainsafe Files](https://files.chainsafe.io/), [web3.storage](https://web3.storage/), [Estuary](https://estuary.tech/) and [Lighthouse](https://www.lighthouse.storage/) for Filecoin, [Satellite Web Interface](https://github.com/storj/storj/wiki/Satellite-GUI) for Storj, [Sia-UI](https://github.com/NebulousLabs/Sia-UI) for Sia)
- Cloud storage rental marketplaces nodes (e.g. [IPFS nodes](https://docs.ipfs.tech/concepts/nodes/#preload), [Filecoin nodes](https://spec.filecoin.io/systems/filecoin_nodes/), [Storj nodes](https://docs.storj.io/node), [Sia hosts](https://docs.sia.tech/hosting/about-hosting-on-sia))

*General description*

Data is uploaded to the chosen decentralized storage network using a compatible client or application. Files are divided into smaller pieces (if necessary), given unique identifiers, and distributed across the network to various storage nodes, each managed by a storage provider or host. Storage agreements or deals are negotiated between the user and storage providers based on the user's requirements regarding data volume, storage duration, retrieval and pricing.

*Filecoin specific description*

Using Filecoin as an example, the general way that storage deals work is that files are imported using the client or application, transformed ([chunked, encoded hashed](https://spec.filecoin.io/systems/filecoin_files/piece/)) into content-addressable representations (CIDs) to locate that data. [Storage deals](https://filecoin.io/blog/posts/how-storage-and-retrieval-deals-work-on-filecoin/) are proposed to Filecoin storage providers using the client or application based on the user’s requirements regarding the amount of data to be stored, storage duration and pricing. The data associated with the CIDs are stored on the Filecoin network by a Storage Provider, and duplicated across the network. If the user wishes to retrieve data associated with CIDs, they can use Filecoin clients or applications to find and propose retrieval deals, either with the same storage provider or dedicated retrieval providers, based on the user’s requirements regarding pricing and retrieval speed (Note: this functionality is still under development, as at the time of writing. See [Saturn documentation](https://docs.filecoin.io/basics/how-retrieval-works/saturn/)). The retrieval provider then locates the data associated with the CIDs in their local storage or on the Filecoin network. Additionally, users who wish to ensure fast access of popular or important data (e.g. in the context of online publishing or app development) may also pin the relevant CIDs to their own IPFS node or delegate this task to a pinning service as a form of “hot storage”.

**Stakeholders involved:**

- Users, organizations or institutions as data providers and potentially data consumers
- Node operators in storage marketplaces as storage and retrieval providers
- Audiences that the user wishes to share their data with as data consumers

**Example of where this pattern is used today:**

Decentralized storage solutions that leverage marketplaces can be used by public institutions to back up large volumes of data as a more resilient and in some cases cheaper approach to digital preservation in place of, or in addition to, centralized approaches.

**Case study:** 

The Internet Archive has partnered with the Filecoin Foundation to back up its archive of internet content on Filecoin.

Read more here: [https://blog.archive.org/2021/04/01/filecoin-foundation-grants-50000-fil-to-the-internet-archive/](https://blog.archive.org/2021/04/01/filecoin-foundation-grants-50000-fil-to-the-internet-archive/)

Web3 platforms that deal with large volumes of data, such as asset-heavy blockchain games or blockchain music streaming platforms also rely on market-based storage solutions to store their data.

**Case study:**

Audius is a streaming music system that connects artists directly to their fans, and uses IPFS and Filecoin to store the content uploaded to its platform.

Read more here: [https://blog.ipfs.tech/2022-02-10-ipfs-filecoin-impact-on-music-media-culture/](https://blog.ipfs.tech/2022-02-10-ipfs-filecoin-impact-on-music-media-culture/)

**Potential challenges:**

The complexity of managing decentralized storage solutions when working with multiple marketplaces and providers may require dedicated resources and expertise in decentralized storage technologies.

Organizations must be prepared to handle [potential fluctuations in storage costs,](https://filecoin.io/blog/posts/the-economics-of-storage-providers/) as these are subject to market dynamics. Websites are available (such as Filfox and Fgas.io) as a source of information that can help an SP’s decision-making process.

Though organizations can negotiate their desired retrieval times as part of retrieval deals, the  retrieval times on offer may be slower than those possible with centralized storage solutions. This capability is still under development for Filecoin (as at time of writing in Q1, 2023. See [Saturn documentation](https://docs.filecoin.io/basics/how-retrieval-works/saturn/)).

**Practices for implementation:**

Organizations may choose to work with multiple marketplaces to optimize storage costs and data resiliency.

**Other contexts where this pattern could be implemented:**

This pattern could be applied in the context of public data sets, for example, for citizen science projects to enable organizations and researchers to store and share large volumes of open data; or media and entertainment platforms that host user-generated content, such as videos, podcasts, or articles, ensuring long-term accessibility and availability.

**Links:**

[https://docs.filecoin.io/store/overview/start-storing/](https://docs.filecoin.io/store/overview/start-storing/)

[https://www.techtarget.com/searchstorage/tip/Comparing-4-decentralized-data-storage-offerings](https://www.techtarget.com/searchstorage/tip/Comparing-4-decentralized-data-storage-offerings)

[https://filecoin.io/blog/posts/the-economics-of-storage-providers/](https://filecoin.io/blog/posts/the-economics-of-storage-providers/)

**Suggested tags:** Persistence, Public Data, Cultural Data, Organizations, Platforms

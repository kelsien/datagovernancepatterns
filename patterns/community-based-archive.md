**Title:** Community based archive

**The need:** 

A local group, organization or institution seeks to store data and make it accessible to a specific set of stakeholders, retaining control and transparency around who stores, accesses and uses the data.

**The solution:** 

Rather than using centralized cloud storage, or decentralized file storage marketplaces, the storage provider may be abstracted or unknown, in a different region or legal jurisdiction to the organization, or simply not in a trusted relationship with the organization, a community-based approach to storage allows organizations to use decentralized data storage solutions within a constrained network of actors that they know and trust.

**Technologies used:**

- [IPFS Cluster](https://docs.ipfs.tech/install/server-infrastructure/)
- Decentralized access control protocols (e.g. [Lit Protocol](https://litprotocol.com/)) or proprietary token-gated dApps (e.g. online platforms, browser extensions, mobile applications)
- Decentralized ordering, time-stamping and logging to blockchains (e.g. [Ceramic](https://ceramic.network/), [Hedera Consensus Service](https://hedera.com/consensus-service))

Data is content addressed using IPFS and stored on a trusted set of nodes as part of an IPFS cluster. Permissions for who can use the data may be controlled by access control protocols, and data events and interactions may be additionally time-stamped and logged to a blockchain for added transparency.

**Stakeholders involved:**

- The organization as the data producer and storage provider
- Partner organizations as storage providers and data consumers
- Other audiences that the organization wants to share their data with as data consumers

**Example of where this pattern is used today:**

Community-based archives are being utilized by activist groups, local cultural institutions, and smaller organizations to preserve and share their resources with a specific audience while retaining control over their data, which may be culturally or context specific, such as the [Omnilingo](https://github.com/omnilingo/omnilingo) local language listening comprehension tool.

**Case study:**

Shift Collective is designing an early prototype for community-centered long-term storage, combining IPFS and Filecoin with their Historypin platform as the front-end interface. They intend to work with 5 community-based archives and their collections, in collaboration with invited institutional partners.

Read more here: [https://www.shiftcollective.us/ffdw](https://www.shiftcollective.us/ffdw)

**Potential challenges:**

Ensuring data security and privacy, while preventing unauthorized access to sensitive information. Maintaining the integrity and availability of data, especially as the size of the archive grows.

Balancing diverse stakeholder needs and expectations while maintaining the archive's overall objectives, and developing a data governance system that allows for the expression of different perspectives may prove challenging.

**Practices for implementation:**

Establish clear and granular access control policies based on roles, attributes, or specific conditions to regulate access, editing, and management of sensitive data within the community-based archive.

Create a robust security framework that includes regular monitoring, vulnerability assessment, and threat mitigation to protect the community-based archive from potential risks and data breaches.

Provide training and resources to storage providers and other stakeholders involved in the archive to ensure they understand their responsibilities with respect to handling sensitive data and maintaining security best practices.

Define a data governance structure that includes guidelines on data classification, retention, and deletion, as well as procedures for handling data breaches or other security incidents.

Conduct regular audits and reviews of the community-based archive to ensure compliance with data protection regulations, access control policies, and security best practices, as well as to identify areas for improvement.

**Other contexts where this pattern could be implemented:**

In the healthcare sector, where patient data needs to be shared within a specific network of healthcare providers while maintaining privacy and security. In educational institutions, where teachers and students need to access and share learning resources within a restricted network. In local government settings, where sensitive documents and data must be shared securely among officials and authorized personnel.

**Links:**

[Shift Collective](https://www.shiftcollective.us/ffdw)

**Suggested tags:** Local, Sensitive Data, Governance

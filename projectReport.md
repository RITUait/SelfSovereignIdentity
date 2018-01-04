##Project report
#Title : **SELF-SOVEREIGN IDENTITY SYSTEM**

##ABSTRACT

Self-Sovereign​ ​ Identity(SSI)​ is ​be​ ​a ​secure,​ ​easy-to-use​ ​system​ ​for​ self-sovereign​ ​identity,​ ​built​ ​on​ ​Ethereum.​ ​It​ ​will consist​ ​of​ ​three​ ​main​ components:​ ​smart​ ​contracts,​​ ​and​ ​a ​DApp (decentralized​ ​ application).​ The​ wallet​ ​will​ ​hold​ ​the​ ​user’s​ keys.
Ethereum​ ​smart​ ​contracts​ ​form​ ​the​ ​core​ of​ ​the​ ​identity.​ ​Finally​ ​the​ ​developer​ libraries​ ​are how​ ​third​ ​party​ app​ ​developers​ ​would​ ​integrate​ ​support​ ​for​ ​SSI​ ​into​ their​ ​apps.
Self-sovereign​ ​identities​ ​can​ ​take​ ​many​ ​forms:​ ​individuals,​ ​devices,​ ​entities,​ ​or​ institutions.
These​ ​identities​ ​are​ ​self-sovereign,​ ​meaning​ ​they​ ​are​ ​fully​ ​owned​ ​and​ ​controlled​ by​ ​the creator,​ ​and​ ​don't​ ​rely​ ​on​ ​centralized​ ​third-parties​ ​for​ ​creation​ ​or​ ​validation.​ ​ A ​core​ ​function​ ​of a​ ​SSI​ ​is​ ​that​ ​it​ ​can​ ​digitally​ ​sign​ ​and​ ​verify​ ​a ​claim,​ ​action,​ ​or​ transaction​ ​- ​which​ covers​ ​a wide​ ​range​ ​of​ ​use​ ​cases.

##CHAPTER 1 : INTRODUCTION

### Introduction to Project

Identity is the most basic requirement of a person in modern society. It is a provision of mutual trust between persons or person and organization. Today, nations and corporations confuse driver’s license, passports, and other state-issued credentials with the identity of an individual. This is extremely problematic because a person can lose his identity if a state revokes his credentials, or if he crosses geographical borders.
Identity in the digital world is an equally tricky ball game. It suffers from the problem of control by centralized authorities, and also because, digital identity varies from one internet domain to another.
It is necessary to redefine the very concepts of digital identity in the modern, overly-digitized world.

### 1.2 Motivation
Not a long time ago, a cryptocurrency called Bitcoin was introduced, with a promising underlying technology called Blockchain[1]. This new technology, which is the basis of Bitcoin, can be used in different other use cases because of its promising features. It can be seen as distributed storage that ensures integrity of the data and solves an integral trust issue. A Blockchain consists of a cryptographically linked list of blocks, which allows only to append blocks. New blocks are added and linked after they have been verified from Blockchain nodes in the network. This process ensures the integrity because blocks in the Blockchain cannot be changed.
Every day we are using more and more online services. This is enabled by the fast
developing IT technology. To be able to access these services we are using digital
identities, which are simplified digital representations of ourselves. This digital identityconsists of a set of attributes related to an identity. Identity management manages those digital identities and their corresponding data. It was further developed through different stages. One of the promising identity management models is the user centric model. In this identity model, the user’s identity data are stored in the user’s domain. The identity models come with certain issues such as there is always trust to a central authority required. Transparency cannot be fully provided, since there is a trusted authority involved. These issues can play an important role in certain use cases, which leads to the conclusion that a new identity model for these use cases has to be developed.

###1.3 Aim and Objectives
Identity management built on the  promising blockchain technology would enable an identity model, which reduces the previous issues for certain use cases. This work introduces Self-Sovereign identity (SSI), a new identity management model. This identity model tries to remove the trust issue that comes with identity management. Moreover, SSI also tries to give the user full control over his/her own data. In this work, we introduce the term Self -Sovereign identity and derive requirements from it. The identified requirements are used to define criteria, which are used to evaluate related Blockchain technologies. Finally, we recommend the most promising technology to realize a SSI system.


##CHAPTER 2 : LITERATURE SURVEY

###2.1 Self-Sovereign Identity (SSI)
The increasing everyday usage of different online services requires an efficient digital identity management approach, especially regarding sensitive personal data. Many people are concerned about how these sensitive data are being managed in terms of where these data are stored and who can access it. Thus, identity management becomes more and more important. Different identity models evolved during time triggered by the increasing demand of online services as well as the further development of those services.
The four main identity models are as follows:
####Isolated Identity Model
The evolution of identity models started with the isolated identity model, which is still the most common model. Its main concept expresses the combination of the Service Provider (SP) and the Identity Provider (IdP), which means that the SP manages the user’s identity data as well as their credentials. In this case, the user authenticates herself directly at the SP.
####Central Identity Model
In contrast to the isolated model, the central identity model separates the IdP from the SP. This separation is the main difference and advancement because the identity data are stored at the IdP. When a user wants to access an online service, she has to first authenticate herself at the IdP and afterwards the identity data are transferred to the SP. In this model, the user does not have any control over her own identity data. An example for this is Facebook because the user does not have control over her own data stored at Facebook.
####User-Centric Identity Model
The user-centric model differs from the central model in storing the user’s identity data in the user’s domain. This domain could be a secure token such as a smart card. Sharing identity data of a user requires explicit user consent. OpenID offers an example. A user can theoretically register his own OpenID, which he can then use autonomously.
####Federated Identity Model
The federated identity model differs from the previous defined models by distributing identity data across multiple IdPs instead of storing it in one central place. In this model, multiple IdPs provide the required identity data to access a service. These IdPs are working together in a federation, which requires a trust relationship between the IdPs. Federated IdPs share a user’s common identifier. This model can be used to realize Single-Sign on (SSO). SSO would be the authentication subset of federated Identity Management.

###Self-Sovereign Identity as the Future
The next further stage of identity models is the Self-Sovereign identity (SSI) model. In this model, the user fully owns and controls her own data. A SSI system creates new requirements on the technology that is used to create such a system. The blockchain technology fulfills most of these requirements. The blockchain technology is described in section 2.1.

###2.2 Blockchain / Distributed Ledger
The blockchain was introduced by Satoshi Nakamoto[2] as part of the peer-to-peer cryptocurrency, Bitcoin. If a user wants to use Bitcoin, she has to install a wallet on her device. The user manages his account using this wallet. Additionally, the user can make transactions such as buying goods and paying with Bitcoin using her wallet. To perform such a transaction, the user has to transfer the right amount of bitcoins to the seller. Bitcoin utilizes the blockchain technology as transaction register to keep record of all bitcoin transactions. Figure 1. Blockchain and its Blocks Architecture shows the blockchain architecture. A blockchain is a cryptographically linked list of blocks where each block consists of transactions, the hash value of the previous block and a nonce. A transaction consists of input and output amount of bitcoins as well as the address of the sender and receiver. Bitcoin uses public key cryptography where the public key represents the address of a user. Bitcoin is a public-permissionless blockchain, which means that anybody can host a copy of the Bitcoin blockchain. Special self-appointed entities of the Bitcoin peer-to-peer network, so-called miner, collecting transactions and try to solve a crypto graphical problem. Solving this problem serves the proof-of-work that ensures the validity of the transactions in the block. The cryptographic problem of the proof-of-work consists of finding the right hash value of a block that starts with the predefined prefix. Miners are using special hardware to calculate the hash values. A nonce is added to the calculation and increased each time another hash results. To calculate the proof-of-work, a few quintillion hash values or even more have to be calculated[3]. After the proof-of-work was successfully calculated, the miner broadcasts the block to the p2p network. Every miner in the network verifies the calculation and if it is correct, the block is added to the blockchain. This approach increases thetransaction security because the whole block is verified. Additionally, the blockchain solves a general trust issue. Different independent miners are verifying a new block, which solves a general trust issue. There is no trust relationship between the different miners required.

Figure 1. Blockchain Architecture


###2.3 Ethereum

Ethereum[4] provides a platform to build decentralized applications with an abstract underlying foundational layer of a blockchain with a built-in Turing-complete programming language, allowing users to write smart contracts[5]and decentralized applications where they can create their own arbitrary rules for ownership, transaction formats and state transition functions.

Figure 2. Ethereum Accounts
###   2.4 Smart Contracts
A smart contract is a computer protocol/program, which automatically executes the contractual part corresponding to the condition that is fulfilled. With smart contracts, you are looking at an incorruptible system of enforcing contracts, thus eliminating the risks of delayed payments and bringing down the risk of non-performance by over 80%.
###2.5 Ethereum Wallet
The Ethereum wallet acts as a gateway for DApps or Decentralized Applications that work on the Ethereum Blockchain. It holds ether, amongst other crypto-assets that are built using Ethereum. Smart contracts can also be written and deployed using the Ethereum wallet.
###2.6 Solidity
Solidity is a programming language used to write smart contracts to run on the Ethereum blockchain. It is a high level language which when compiled gets converted to EVM (Ethereum Virtual Machine) bytecode; similar to the world of Java where there are JVM languages like Scala, Groovy, Clojure, JRuby etc and on compilation generate byte code which run in the JVM (Java Virtual Machine).

###2.7 Permissionless (Public) / Permissioned (Private) Blockchain
This criterion describes if the Blockchain is public or private. The difference here is that either everybody can or cannot access the Blockchain with or without permission. Both permissioned and permissionless blockchains have advantages and disadvantages. On the one hand, permissionless (public) blockchains prove the consensus of the data with the proof-of-work. This proof usually consists of solving a cryptographic problem. Special entities (miner) try to solve this problem because they receive a commission after successfully solving the problem. The arising problem is to motivate the miner to solve this problem, which is the received commission. Many independent miners are trying to receive the commission by solving the proof-of-work. Therefore, no trust relationship between the parties is required. On the other hand, the advantage of using a permissioned blockchain is that the proof-of-work does not have to be a difficult to solve cryptographic problem, i.e. transactions can be confirmed within a short timeframe. The need for motivating the miner with commissions is not required. As disadvantage can be seen that the permissioned entities have to be semi trusted or at least the authority, which decides if an entity becomes an authorized entity with write-access to the ledger.


##CHAPTER 3 : REQUIREMENT ANALYSIS

###3.1 Problem Statement
Using Self-sovereign identity people and organisations can store their own digital identity on their own devices, and provide it efficiently to those who need to validate it, without relying on a central repository of identity data. Self-Sovereign Identity (SSI) is an identity that is fully owned and controlled by an individual or organization. No one else can read it, use it, or take it away without its owner’s explicit consent.
###3.2 Benefits
The stakeholders of a SSI system are citizens, public administration and businesses. From a citizen perspective, a SSI system would give the citizens power to fully own and control their own identity data. Furthermore, trust in a single authority is not necessary anymore. Security and privacy will be maintained. The citizen only decides what kind of data are going to be stored in the ledger and who is going to access it. For example, if a SSI system is deployed in the whole European Union, it can be utilized for cross-border authentication and for cross border services. A SSI system provides the citizens a platform to use their electronic identity all the time and everywhere. Such a SSI system is also beneficial for the government. It could help decrease costs related to identity management. Additionally, a SSI system offers full transparency in the identity management, which can help to increase the citizen’s trust in the government. In addition, cross border government processes and services can be easily realized. Businesses can benefit from a SSI system when providing services and a qualified identity provider is required. It can save time and costs for the companies.



###3.3 Challenges
When applying a SSI model, various challenges arise such as access permission level of the blockchain, proof of work calculation, missing technical understanding and data storage issues.
The access permission level of the blockchain depends on the chosen technology. This can vary between public (permissionless) to private (permissioned) access permission level. Using a public blockchain requires the proof-of-work calculation to ensure secure and tamper resistant consensus. This proof-of-work requires huge amount computation power. In contrast, using a private blockchain requires trust in the parties that are responsible for writing and reading data from or to the ledger.
Another obstacle when using SSI model can be the missing technical understanding of this novel technology. This lack of knowledge can lead to problems such as integration issues when trying to integrate a SSI model into existing infrastructure.
Utilizing SSI emerges data storage issues especially when storing sensitive data. Some blockchain implementations are using additional external storage. When the sensitive data are stored encrypted in the blockchain key distribution problems arising. The limited storage capacity of blockchains describe another storage issue.


##CHAPTER 4: PROPOSED DESIGN

###4.1  Permissionless (Public) / Permissioned (Private)
SSI is a permissioned distributed ledger. The SSI foundation defines nodes, which are both authorized and responsible for reading and writing from and to the distributed ledger. SSI defines two types of nodes that are responsible and authorized for read and write operations to the ledger. The observer nodes are responsible for the read operations from the ledger  and the validator nodes handle the write operations. Additionally, the observer keep the ledgers synchronized between them and the observer nodes.
###4.2 Proof-Of-Work (Mining)
This technology uses a distributed consensus protocol named Plenum Byzantine Fault Tolerant Protocol . This open source protocol–developed by Evernym-is optimized for security and scalability. Because the ledger is permissioned, a difficult computation to calculate the proof-of-work is not required.
###4.3 Key management system
The keys are stored in a decentralized public key infrastructure (DPKI). An identity owner uses keys, which are stored in a keychain. The keychain itself is stored in a DPKI.Approaches for key discovery, rotation and revocation and recovery are defined. Identity Data Import / Gathering. The imported identity data have to fulfill the SSI data format. Additionally, to be able to apply selective disclosure, each identity attribute has to be individually signed.
###4.4 Selective Attribute Disclosure Support
SSI supports selective disclosure of identity attributes. The imported attributes have to fulfill the SSI format. If authenticity is required each attribute has to be individually signed.
###4.5 Data storage
SSI offers two different storage options: the on-or off-ledger storage. Identity data, keys, transaction proofs an pointers are stored on-ledger. Other digital data can be stored off-ledger. Nevertheless, multiple factors influence the decision what kind of data are stored on-or off-ledger.
##4.6 Trust Required
The board of trustees governs SSI as well as decides and approves who is going to be a steward. A steward is a trusted entity, which is performing operations on the ledger. Stewards take the role of observer and validator node. Therefore, trust in the SSI foundation and their decisions is required.
###4.7 Identifiers
SSI uses key-value pairs to identify each identity owner on the ledger[6]. Decentralized identifiers (DIDs) are the key and DID description objects (DDOs) are its associated value. These key-value pairs are called DID record. The design of DID records removes the dependency on a central authority.

Figure 3. Use Case Diagram

Figure 4. SSI DApp Architecture

##CONCLUSION
The architecture of a Self-Sovereign identity system based on the blockchain technology is described as follows. The blockchain offers the possibility to realize a system without semi-trusted parties such as central certificate authorities (CAs) or registration authorities (RAs). Nevertheless, the degree of required trust depends on the specific blockchain implementation. Only public or permissionless blockchains provide a fully semi-trust less environment. If a blockchain is private or permissioned, only authorized parties have access to the ledger, which requires at least some kind of trust relationship to these entities. Even though authorized parties are independent of each other, trust in the chosen parties or in the selection process of becoming a trusted party is still necessary. Independent authorities should host a copy of the ledger that helps reducing the required trust. These authorities can be for example different countries of the European Union. The citizen of a country A could then import their identity data using the existing eIDAS infrastructure. eIDAS nodes are used to import qualified identity data into the user’s ledger. A citizen should be able to use her smart phone to access or share her identity data wherever they want where each identity’s data access is logged. The blockchain ledger is the central part of such a SSI system. Nevertheless, there are additional parts required to fully support all features and use cases which are described . Therefore, the distributed ledger has to be extended by at least two additional parts namely the off-ledger storage and the data import part.


##REFERENCES

[1]  http://nakamotoinstitute.org/bitcoin/
[2] http://gavwood.com/paper.pdf
[3] https://github.com/ethereum/wiki/wiki/White-Paper
[4] https://whitepaper.uport.me/uPort_whitepaper_DRAFT20170221.pdf
[5] https://tokensale.civic.com/CivicTokenSaleWhitePaper.pdf
[6] https://sovrin.org/library/
[7] http://id2020.org/

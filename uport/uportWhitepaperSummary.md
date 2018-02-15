# Whitepaper Summary

##UPORT: A PLATFORM FOR SELF-SOVEREIGN IDENTITY
##INTRODUCTION
####History
There are many problems with the current state of identity systems. Digital identity is fragmented and siloed between various servi
ce providers, prohibiting a holistic view, and delivering poor user experience
necessitating repetitive registrations and logins with usernames and passwords. This results in insecure
systems where people use th
e same password for m
any of their sites. The centralized servers of identity
providers like Google and F
acebook are honeypots of data, so they’re economically valuable for hackers
to attempt to crack. The upcom
ing reliance on billions of internet-of-things devices makes it untenable to
have all those devices contr
olled by a centralized identity provider, since a breach of this provider would
prove catastrophic to not on
ly digital but also physical infrastructure.
Public/private key cryptogra
phy and decentralized technologies like blockchains offer a promising
solution to the problems me
ntioned above. These technologies push ownership of identity away from
centralized services to the edge
s - to individuals - so that the identities themselves are in control. This is
commonly referred to as
​
 sel
f-sovereign i
dentity
​
. This approach decentralizes data and computation and
pushes them to the edges, w
here it is less economically valuable to hackers because it would require a lot
of effort to hack many indiv
idual identities one-by-one
.
However, introducing new t
echnologies to end-users is difficult. Public-key cryptographic tools like 
​
PGP
have been around for 25 yea
rs, but their use in digital identity systems have seen little use due to their
unintuitive and complex use
r experience, and the fact that usernames and passwords work well enough
for most people. Blockchain
 technologies are interesting in that they 
​
requi
re
​
 the use of cryptographic keys
to sign messages for each int
eraction of the blockchain. Thus the rise of cryptocurrencies like Bitcoin and
general blockchain architec
tures like Ethereum have sparked new interest in making publ
ic key
cryptography usable to regu
lar consumers and users in order for them to interact with these systems.
Interactions with blockchain
 based systems necessitate usable public-key cryptography, and up to this
point the key management s
olutions (commonly called “wallets”) have been difficult to use for
non-technical users. Interest
ingly the blockchain can itself help make public-key cryptography more
usable and secure by acting
 as a decentralized public key infrastructure (PKI). The blockchain can be
viewed as a decentralized c
ertificate authority that can maintain the mapping of identities to public keys.
Smart contracts can furtherm
ore add sophisticated logic that helps with key revocation and recovery,
lessening the key manageme
nt burden for the end user.
Introduction to Uport
Uport is a secure, easy-to-u
se system for self-sovereign identity, built on Ethereum. The uPort technology
consists of three main compone
nts: smart contracts, developer libraries, and a mobile app.
The mobile app holds the use
r’s keys. Ethereum smart contracts form the core of the identity and contain
logic that lets the user recove
r their identity if their mobile device is lost. Finally the developer libraries
are how third party app dev
elopers would integrate support for uPort into their apps.
uPort identities can take ma
ny form
s: individuals, devices, entities, or institutions. Uport identities are
self-sovereign, meaning the
y are fully owned and controlled by the creator, and don'
t rely on centralized
third-parties for creation or va
lidation. A core function of a uPort identity is that it can digitally sign and
verify a claim, action, or trans
action - which covers a wide range of use cases.
An identity can be cryptogr
aphically linked to off-chain data stores. Each identity is capable of storing the
hash of an attributed data bl
ob, whether on 
​
IPFS
​
, Azure, AWS, Dropbox, etc., which is where all data
associated with that identity
 is securely stored. Identities are capable of updating this file themselves, such
as adding a profile photo or
 a friend, or they can also grant others temporary permission to read or write
specific files.
Since they can interact with
 blockchains, uPort identities can also control digital bearer assets such as
cryptocurrencies or other to
kenized assets.
Proposed Use Cases
A self-sovereign identity sys
tem will have many use cases, here a few of them are presented:
uPort allows end-users to: o
wn and control their personal identity, reputation, data, and digital assets;
securely and selectively dis
close their data to counterparties; access digital services without using
passwords; digitally sign cla
ims, transactions, and documents; control and send value on a blockchain;
interact with decentralized a
pplications and smart contracts; and encrypt messages and data.
uPort allows enterprises to: e
stablish a corporate identity; easily onboa
rd new customers and employees;
establish an improved and t
ransitive Know-Your-Cus
tomer process; build secure access-controlled
environments with less fricti
on for e
mployees; reduce liability by not
 holding sensitive customer
information; increase compl
iance; maintain a network of ve
ndors; establish role-specific, actor-agnostic
identities (i.e. CTO) with spe
cific permissions.
TECHNICAL OVERVIE
W


Publicly Verified Blockchain Identity for Autonomous Educational Institutions

A live implementation of a Self-Sovreign Institution issued identity on Ethereum. The initial aim is to have 300 students of Army Institue of Technology have successfully verified their uPort identity in person with the College, enabling them to access a new suite of autonomous institute  services in a trusted and self-reliant manner. 
How it works: Mechanics of the AIT ID

Alice is a student of AIT and enrolls in the AIT digital identity system. She downloads the AIT ID app from the App Store and creates an account. In this moment, the AIT app creates a unique private key on her phone and deploys two smart contracts on the Ethereum network that act as the user’s identity hub (currently identities are being deployed on public testnet Rinkeby, however Main-net support will follow soon).

More specifically, Alice’s private key manages a controller contract, which allows her to recover access to her identity should she lose access to her phone. The controller contract in turn controls her identity (proxy) contract, or permanent identifier. With this setup, Alice is now in complete control of her identity and all its associated data and can’t lose access due to loss of her private key.
Basic uPort Architecture Overview

After around 2 minutes, Alice has created her AIT ID on the public Ethereum network and may now visit the website of College to register. Here, she scans a QR code to interact with the identity of the College for the first time. The College has its own identity on a public Ethereum network that allows it to sign and verify data.

Access to the College identity is managed by the College clerk, who uses their own personal AIT ID identity authorized with specific admin rights. 

Once Alice has entered her date of birth and permanent registration number on the City website, her request is cryptographically signed and sent to the College as a new verification request. She is asked to visit the College’s registration office for an in-person verification of her details within 14 days. Once confirmed, the College clerk issues Alice a verified attestation that is signed by the College’s identity, as a server-side credential.

Alice is now able to interact with the online services of the College in a seamless way. She doesn’t need a user account or password to log-in, and with each interaction she does, the college  knows exactly who it’s dealing with. Whenever she logs into the Colleges’s web portal, a “Requester server” validates that the identity who provides the attestation is the same identity that received the previous attestation. You can read more about the inner workings of our server side attestations and review a guide to set up your own app identities here.
__First Use Cases and Next Steps__

Another use case that is being discussed is an integration with the fees web portal. Here, the eID could be used to identify yourself when logging into the fees portal, submit your forms and receive a corresponding ticket or timestamped attestation of submission.
Alice could submit all her assignments online and digitally sign the submission with her AIT ID!

These examples show that a once-issued attestation like this can be used by a multitude of service-providers, dapps, and government agencies, and can potentially greatly decrease the cost of on-boarding and compliance.

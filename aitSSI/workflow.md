1. Instantiate the uPort object:

const uport = new Connect('NAME_OF_DAPP', {
  clientId: 'CLIENT_ID',
  signer: SimpleSigner('SIGNING KEY')
})

clientId - public address of the app
signer - signing key of the app	

Note: Register your app with the uPort App Manager to receive these details.

2. Request Specific Credentials:

uport.requestCredentials({
  requested: ['name', 'avatar', 'phone', 'country'],
  }).then((userProfile) => {
    // Do something after they have disclosed credentials
})

The expected payload (userProfile) looks like this, when requesting all credentials - 

{
  "@context":"http://schema.org",
  "@type":"Person",
  "name":"Agent Smith",
  "address":"23fga3r2hh87ddhq98dhas8dz101j9f449w0",
  "avatar": {
    "uri": "https://ipfs.infura.io/ipfs/QmaqGAeHmwAi44T6ZrSuu3yxwiyHPxoE1rHGmKxeCuZbS7DBX"
  },
  "country": "US"
  "network":"rinkeby",
  "publicEncKey": "dgH1devHn5MhAcph+np8MI4ZLB2kJWqRc4NTwtAj6Fs="
  "publicKey":"0x04016751595cf2f1429367d6c83a826526g613b4f7574af55ded0364f0fb34600bceba9211e5864ae616d7e83b5e3c79f1c913b40c8d38c64952fef383fd3ad637",
}

3. Enable Push Notifications: 

If the notifications flag is set to true it will allow any future transaction signing to fire a prompt in the uPort mobile app, otherwise users will have to scan a QR code per each interaction.

uport.requestCredentials({
  requested: ['name', 'avatar', 'phone', 'country'],
  notifcations: true
  }).then((userProfile) => {
    // Do something after they have disclosed credentials
})

4. Attesting Credentials:

uport.attestCredentials({
  sub: 'THE_RECEIVING_UPORT_ID',
  claim: { CUSTOM_PROPERTY: PROPERTY_VALUE },
})

We can also set an expiry date for the credentials to persist until - 

uport.attestCredentials({
  sub: 'THE_RECEIVING_UPORT_ID',
  claim: { CUSTOM_PROPERTY: PROPERTY_VALUE },
  exp: new Date().getTime() + 30 * 24 * 60 * 60 * 1000,  // Optional expiration
})

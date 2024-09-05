# FAQs

### Where are VC’s data stored?

Credential data are encrypted and stored in an organised format on KwilDB (a decentralised fault-tolerant database). Using a db like Kwil over a file system like IPFS and Irys for storing encrypted credentials gives us flexible access to fetching the overarching data, and filtering data for decryption and proof generation.

### How are ZKPs recovered for the Marketplace?

After generation ZKPs are stored on Irys and can be fetched to verify public inputs of the ZKP as well as verifying the proof itself. This way proofs and the underlying verified data can be accessed and used through the Marketplace SDK.

### Why use both MPCs and AA, rather than just AA?

Smart wallets require secret authentications, and contracts cannot inherently possess said secret. This means that the security of AA systems are outsourced (this applies to all current standards including multisigs). Sourcing the security and recoverability of AAs to MPC wallets ensure that the key share system is the only thing we need to prioritise. Aside from this, MPC wallets give users the ability to encrypt and decrypt their data on the fly without revealing any underlying secrets.

### How are key shares kept secure?

We’re currently implementing DKG systems to generate key shares among multiple secure enclaves (through dkls23). We’re also considering including Shamir’s algorithm to enable users to import existing EOAs as OMIDs (this however could undermine security, but could benefit from importing already used ID systems like Privado and Anima that are locked to EOAs), and we’re not yet fully decided on this.

\

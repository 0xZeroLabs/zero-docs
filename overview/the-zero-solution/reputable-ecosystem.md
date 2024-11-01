# Reputable Ecosystem

While reputation scoring could undermine censorship resistance, it will ultimately help in identifying maliciously actors on the open web. The current plan is to implement reputation scoring to verify those that try to tamper with their ID data either during the issuance or when in their custody.

Issuance tampering occur when a prover (user) colludes with one of the [S3N](../../developers/s3n.md) nodes in order to pass off fake data as correct one. In such a scenario, both the prover and the node operator will be punished.

* Provers receive a reputation damage. Although this doesn't censor the prover per se, it stands them out to any verifier or basically any other participants of the ecosystem as they might be malicious.
* Node operators of [S3N](../../developers/s3n.md) as with every AVS on [EigenLayer](https://eigenlayer.xyz), get slashed if caught trying to collude. While this might not be a common occurrence, it's important to put in place to ensure a safe ecosystem.

Due to the nature of self-sovereign identities, provers have full control over what data is in their possession and can always modify them. However, malicious modifications should be punished and can be identified when a verifier is presented with a faulty proof trying to validate any provable data given to them.

# Reputable IDs

While reputation scoring could undermine censorship resistance of identities, it can ultimately help to identify those who act maliciously on the open web. The current plan is to implement reputation scores to verify those that try to tamper with their ID data during either the issuance or when in their custody.

Issuance tampering occur when a prover (user) colludes with one of the S3N nodes in order to pass off fake data as correct one. In such a scenario, both the prover and the node operator will be punished.

* Provers receive a reputation damage. Although this doesn't censor the prover per se, it stands them out to any verifier or basically any other person in the ecosystem that they might be malicious.
* Node operators of S3N as with every AVS on EigenLayer, get slashed if caught trying to collude. While this might not be a common occurrence, it's important to put in place to ensure a sage ecosystem.

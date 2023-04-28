# Digital Signatures

Declarations, assertions or claims to the content can be made, in principle, by anyone – regardless of rights or content ownership and without consent of the actual rightsholders.

When claims or assertions to content, ISCCs, metadata, and attribution are published on the Internet, there is no easy way to verify them.

However, when an ISCC is registered on a public blockchain, this happens in the context of a transaction which is public, open, and transparent. The ISCC declaration binds a specific ISCC to the pseudonymous actor originating a blockchain transaction.

Most public blockchain networks are based on asymmetric public key cryptography. This means that transactions on these blockchains usually allow to infer the pseudonymous actor who triggered a transaction by means of his pseudonymous wallet address. This public wallet address is derived from the public key controlled by the user.

To perform a blockchain transaction with a wallet, the user needs to be in control of the corresponding private key; only the private key allows the user to cryptographically sign the blockchain transaction. The fact that there is always a pseudonymous actor that originates the transaction implies that there is always a potentially identifiable user.

A digital signature with a wallet software is the conceptual technical basis and starting point of the Liccium app. It cryptographically proves that a user, who can first and foremost be pseudonymously identified by the wallet address, had access to the corresponding private key.

Digital signatures can only be signed by users controlling the pair of both private and public keys. A malicious actor could not sign a transaction that challenges the legitimate owner of a public key unless the former has obtained access to the private key.

ISCC declarations are decentralised, self-sovereign, permissionless and blockchain-agnostic, which means that users can declare ISCC codes with their own wallet to smart contracts they control on (in principle) any public blockchain network.

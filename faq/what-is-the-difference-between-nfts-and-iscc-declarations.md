---
hidden: true
---

# What is the difference between NFTs and ISCC declarations?

When an NFT is being minted, the issuer is calling the minting function of an NFT smart contract. This function requires certain parameters, like the recipient address, the token ID, and any metadata associated with the NFT.

The NFT metadata, according to the NFT metadata standard, usually contains information about the NFT, such as its name, description, image, and other attributes.

The token ID is a unique identifier assigned to each NFT in a smart contract. It can be used as a parameter in the token URI function to retrieve the metadata associated with a specific NFT. Thereby, the metadata file is linked to the NFT on the blockchain.

To declare an ISCC code – on the other hand –, an application must call an ISCC declaration smart contract on a public blockchain. This transaction provides information about the ISCC code and the URI to the primary declaration metadata, signed by the wallet of the declarer. This information is stored on-chain in the event log of the smart contract and provided to a hub smart contract to mint an ISCC-ID.

Minting an ISCC-ID means that public declarations of ISCC codes on different blockchains are monitored and registered by an off-chain application to calculate and index ISCC-IDs and create a registry based on the events received from the observers.

The token ID of the NFT is provided by the original minter, while the ISCC-ID is calculated post-transaction in an off-chain registry based on the events received from observers.

The URI to metadata of an NFT are stored in the smart contract, whereas the link to metadata of the ISCC declaration is stored in the event log of the blockchain transaction.

In both cases, the metadata file itself is often hosted on IPFS (InterPlanetary File System), which is a decentralised file storage system.

While NFTs may only be relevant for a minority of use cases in digital media distribution and sales, e.g., to offer a unique digital asset or access to other items of value, the benefit of NFT is that it can be easily traded and transferred using existing and established wallet software.

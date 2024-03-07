# Permissionless on-chain declarations

Instead of declaring identifiers, metadata, or rights management information for digital media content to centralised, industry- and sector-specific, regional, national or international registration authorities or copyright offices, permissionless on-chain declarations of ISCC codes on public blockchain networks allow to inseparably link external product and title metadata, rights management information and other information on persistent data repository to make public declarations of claims to the content

The ISCC system provides a protocol for decentralised, cross-chain, content registries that supports a service for the aggregation and discovery of ISCC declarations across different blockchains. This will create a global and publicly auditable registry of blockchain transactions that bind ISCC codes to pseudonymous declarants, claims and assertions.

To declare an ISCC code an application must call an ISCC declaration smart contract on a public blockchain. This transaction provides the string of the ISCC code and the URL to the primary declaration metadata, signed by the wallet of the declarer. This information is stored on-chain in the event log of the smart contract and provided to a hub smart contract to mint an ISCC-ID.

| On-chain Transaction |                                                                                                                                                                                               |
| -------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Transaction Hash     | 0x7de58fb6d3c040d63ee1d085a101fed67eed18434361222d47b0710622777060                                                                                                                            |
| Block                | 8693803                                                                                                                                                                                       |
| Timestamp            | Mar-21-2023 03:16:24 PM +UTC)                                                                                                                                                                 |
| From                 | 0xeb761B8d104E2c573fD0153E3E14b6055338e749                                                                                                                                                    |
| To                   | 0x4E016d1F09a182e8981Ee19FABc8E45D365E5d22                                                                                                                                                    |
| Input Data           | <p>#; Name; Type; Data<br>0; iscc; string; KECRJIIZC5ZHNBZQVMVZPVFWUGA4YXC5RCGZJPUR4QJ6UTIBJ3VKVEY<br>1; url; string; https://ipfs.io/ipfs/Qma8C4ZdvRbcLFxUektvS3VQ32jta2ZCn7vLHCkYWdKfXX</p> |

Source: [https://goerli.etherscan.io/tx/0x7de58fb6d3c040d63ee1d085a101fed67eed1843 4361222d47b0710622777060](https://goerli.etherscan.io/tx/0x7de58fb6d3c040d63ee1d085a101fed67eed18434361222d47b0710622777060)

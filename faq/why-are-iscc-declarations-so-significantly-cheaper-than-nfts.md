---
hidden: true
---

# Why are ISCC declarations so significantly cheaper than NFTs?

Gas costs in the evm-based blockchain are higher for storing data in a contract compared to storing data in an event log because contract storage is a more expensive and resource-intensive operation.

When data is stored in a contract, it is permanently stored on the blockchain and must be processed by every node in the network. The costs associated with the storage and retrieval of data in contract storage are reflected in the gas costs. The gas cost of storing data in a contract is higher because the operation requires more computational resources and has a greater impact on the overall state of the blockchain.

Additionally, event logs are a more lightweight and efficient method of broadcasting information. They do not require any changes to the contract storage, and they are not processed by every node in the network. This means that the gas costs associated with event logs are generally significantly lower than those associated with contract storage.

# What is the difference between contract storage and event log storage on the EVM-based blockchains?

On EVM-based blockchains, contract storage is used to store the persistent state of a smart contract.

An EVM-based blockchain is a key-value database where each smart contract has its own storage without time expiry. The values stored in contract storage can be updated and modified by calling functions within the smart contract. Contract storage is used to maintain the state of the contract and to record important data such as the balance of an ERC-20 token or the number of votes in a decentralised voting system.

Event logs, on the other hand, are a way for smart contracts to emit information about events that have occurred within the contract. Event logs are stored in a separate data structure, separate from contract storage. They are broadcasted to the entire network and synced by all nodes. Event logs are a way to broadcast information to the rest of the network, and they can be indexed and searched by external services, making it possible to easily track events that occur within the contract. They can be used to record events such as a token transfer, a voting decision, or any other type of action that occurs within the contract.

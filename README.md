# awesome-blockchain-sharding
Awesome Assets on Blockchain Sharding Systems

## Introduction
- Sharding aims at dividng the nodes into nodes into different consensus groups that process transactions concurrently.
- A transaction may involve a single shard (called intra-shard transaction) or multiple shards (called cross-shard transaction).
- To process cross-shard transactions, nodes in different shards may communicate with each other.

## Important Layers
- Data Layer :
  - defines how the ledger is formatted and divided into different shards
  - data verification rules are defined in this layer
- Membership Layer :
  - Defines how nodes are allocated to different shards.
  - Shard allocation algorithms are defined in this layer
- Intra Shard Layer :
  - Defines how each shard processes local transactions.
  - Leader election and consensus is defined in this layer.  
- Cross Shard Layer :
  - Defines how shards process cross-shard transactions. 
  - Concurrency control and atomic commit are defined in this layer.
 
## Common Techniques
- Sharding can be broadly classified into the following categories
  - State Sharding :  Shards communicate with each other through a state, or central, relay
  - Partitioned Sharding : Shards don’t communicate with each other directly through a central relay
 
## Existing Implementations
- Ethereum :
  - Beacon chain has implemented sharding. It maintains the set of active, queued and exited validators
  - Beacon chain processes cross links and its own block by block consensus as well as a finality gadget
- Polkadot :
  - Parachains
- NEAR : 
- Ziliqa : 

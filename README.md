# The Aggregation Layer

Aggregated blockchain design borrows the best of the monolothic and modular approaches to scale. In its endstate, the Aggregation Layer will provide a common language for secure, atomic, interoperability among heterogeneous chains.

The Aggregation Layer is a decentralized protocol with two components: a common bridge + the ZK-powered proof validation and aggregation mechanism for seamless, cross-chain transactions. With ZK proofs providing securing chains connected to the Aggregation Layer can remain sovereign and module while preserving the seamless UX of monolithic chains.

## Components

### Unified LxLy Bridge

The Unified LxLy Bridge is the backbone of the Aggregation Layer. It is designed to act as a common way for connected EVM chains to exchange messages and assets safely. Implementations of this bridge for non-evm chains are in progress and will be linked and included when teams have made them available.

[Source Code](https://github.com/AggLayer/ulxly-contracts) | [Documentation](https://github.com/0xPolygonHermez/zkevm-techdocs/blob/main/slides/zkevm-architecture-part5-ulxly.pdf)
### AggLayer v1

AggLayer v1 is a simple system which allows blockchains which are connected to the Unified LxLy bridge to transmit proofs to Ethereum safely. This system is designed primarily to serve CDK chains utilizing full validity proofs with which it acts as security layer, checking proof validity before settling directly to Ethereum.

Source Code: [Golang](https://github.com/AggLayer/agglayer-go), Rust (COMING SOON)

### Bridge and Call

Bridge and Call is a smart contract framework which allows applications to take advantage of the Unified LxLy Bridge and the Aggregation Layer to unlock cross-chain interactions for their application. Using Bridge and Call a user can use funds on a source chain to directly interact with an application running on a destination chain

[Source Code](https://github.com/AggLayer/lxly-bridge-and-call)
## Specification (Coming Soon)

A draft specification describing the decentralized vision of the AggLayer is coming soon. This will be aimed primarily at blockchain developers and integrators looking to understand the principals at work, and will be open for feedback and contribution to the broad community.

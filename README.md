# Formal Verification of Ethereum Smart Contracts with a Proof Assistant
## Motivation
### Security emanates from correctness
### Security bugs are prevalent
### Firms pay a lot to discover security bugs
### Formal verification is the way
#### Why model checkers and SMT solvers are not up to the task
#### Why using a proof assistant is the best approach
## Overview
The formal verification system includes a new language to write smart contracts in. Only contracts written in the new language can be verified in the system. These contracts can be deployed anywhere Ethereum Virtual Machine is supported.

The architecture of the formal verification system is as follows:
- **Input code:** Written in the new language, which is more restricted than Solidity. It is much closer to lower level concepts of the Ethereum blockchain. Notable features are:
  + Only loops where the iteration count is known in advance are allowed
  + Contracts take binary data as input and returns binary data as output
    * In Solidity, even though fundamentally contracts process binary data and return binary data, it has a layer of abstraction over the binary data called the Application Binary Interface
- **Compiler:** Takes code written in the new language and compiles into both Solidity and Coq. The Solidity code can be used to deploy to Ethereum Virtual Machine compatible blockchains, while the Coq code can be used to prove correctness properties.
- **Foundational definitions:** The Coq code cannot stand by itself. It must have some foundational definitions to lean on. The definitions include:
  + Monads
  + Algebraic effects
### Foundational definitions
### Compilation process
### Syntax of new language
### Verification process
## Verified contracts
### Simple contract
### Merge sort
### Heap data structure
### Prime factorization
#### With reentrancy bug
#### Without reentrancy bug
### Binary search

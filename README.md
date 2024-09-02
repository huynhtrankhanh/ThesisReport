# Formal Verification of Ethereum Smart Contracts with a Proof Assistant
## Motivation
### Security emanates from correctness
### Security bugs are prevalent
### Firms pay a lot to discover security bugs
### Formal verification is the way
#### Why model checkers and SMT solvers are not up to the task
#### Why using a proof assistant is the best approach
## Overview
The architecture of the formal verification system is as follows:
- **Input code:** Written in a new language, which is more restricted than Solidity. It is much closer to lower level concepts of the Ethereum blockchain. Notable features are:
  + Only loops where the iteration count is known in advance are allowed.
  + 
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

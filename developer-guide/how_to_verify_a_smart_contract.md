---
title: How To Verify A Smart Contract
---

This how to shows the steps you need to follow to verify a smart contract through a flattened source code.

## Prerequisites

1. The smart contract address, let us assume it is `SMART_CONTRACT_ADDRESS`
2. The compiler version used to compile the smart contract, let us assume it is `COMPILER_VERSION`
3. The EVM version for which the WASM was compiled for, let us assume it is `EVM_LONDON`
4. The solidity flattened sources file for your smart contract

## Start

Go to https://trustscan.one/address/SMART_CONTRACT_ADDRESS/verify-via-flattened-code/new

## Fill In The Verification Form

1. Select the compiler version used to compile the smart contract, in this case the `COMPILER_VERSION`
2. Select the EVM version, in this case `EVM_LONDON`
3. Fill in the solidity contract flattened code
4. Click `Verify & Push` button.

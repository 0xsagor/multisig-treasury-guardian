# MultiSig Treasury Guardian

An expert-level smart contract solution for managing organizational funds with decentralized security. This repository provides a robust "m-of-n" signature logic, ensuring that no single individual can move funds without a consensus from authorized signers.

## Features
* **Customizable Quorum**: Define the number of required signatures (e.g., 3-of-5).
* **Transaction Queue**: Proposals are stored on-chain until the threshold is met.
* **ERC20/ETH Compatibility**: Supports both native currency and token transfers.
* **Guardian Role**: An optional recovery mechanism for resetting lost signers.

## Technical Workflow
1. **Submit**: Any signer proposes a transaction.
2. **Confirm**: Other signers provide approvals via their private keys.
3. **Execute**: Once the threshold is reached, anyone can trigger the execution.

## Setup
* Edit the initial signers array in the deployment script.
* Deploy to any EVM-compatible chain (Ethereum, Polygon, Arbitrum).
* Use the provided frontend-ready JSON ABI for integration.

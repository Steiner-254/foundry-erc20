# ERC20 Token Project

This repository provides a framework for developing, deploying, and testing an ERC20 token on the Ethereum blockchain using Foundry, a fast, portable, and modular toolkit for Ethereum applications. This project includes all necessary components for ERC20 token management, automated testing, and CI/CD integration for continuous delivery.

---

## Table of Contents
- [Overview](#overview)
- [Project Structure](#project-structure)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Configuration](#configuration)
- [Compiling Contracts](#compiling-contracts)
- [Deployment](#deployment)
- [Testing](#testing)
- [Scripts](#scripts)
- [Troubleshooting](#troubleshooting)
- [License](#license)

---

## Overview

This project provides an ERC20 token implementation with customization options to meet various tokenomics requirements, making it suitable for decentralized applications (DApps), financial ecosystems, and smart contract applications. The primary tools used are:

- **Foundry**: A Solidity toolkit for compiling, testing, and deploying contracts.
- **Forge**: Foundry's testing framework.
- **GitHub Actions**: Integrated for automated testing and deployment workflows.

## Project Structure

The repository is organized as follows:

```javascript
├── .github/workflows # CI/CD workflows for automated testing and deployment ├── lib # External libraries and dependencies ├── script # Deployment and contract interaction scripts ├── src # Smart contract source code │ └── ERC20.sol # ERC20 contract implementation ├── test # Unit and integration tests ├── .gitignore # File to ignore specific files in git ├── .gitmodules # Defines any git submodules ├── Makefile # Makefile for commonly used commands ├── README.md # Project documentation └── foundry.toml # Configuration file for Foundry
```


## Prerequisites

Ensure you have the following tools installed on your system:

1. **Foundry and Forge**: Foundry is used for Ethereum smart contract development. [Installation instructions](https://book.getfoundry.sh/) are provided on Foundry’s documentation page.
2. **Node.js and npm**: For managing dependencies and additional scripts. You can download Node.js from [here](https://nodejs.org/).

## Installation

1. **Clone the repository**:

   ```bash
   git clone <repository-url>
   cd foundry-erc20
   ```

2. **Install Foundry and Forge:**

- If Foundry is not installed, use the following commands:

   ```bash
   curl -L https://foundry.paradigm.xyz | bash
   foundryup
   ```


3. **Install additional dependencies (if any are required):**

   ```bash
   npm install
   ```


# Configuration
1. **Edit Environment Variables:** Update the configuration file, typically foundry.toml, with network details, such as RPC URL and private keys, for deployment.

```toml
[default]
rpc_url = "<YOUR_RPC_URL>"
private_key = "<YOUR_PRIVATE_KEY>"
```

2. **Update Deployment Script:** Modify any deployment parameters in the deployment script under `script/`.


# Compiling Contracts
- To compile the smart contracts, execute:

```bash
forge build
```

- If the compilation is successful, you should see Compiled successfully in the output.


# Deployment
- Use Foundry's script functionality to deploy the contract to a specified network. Make sure your foundry.toml file has the correct RPC URL and private key settings:

```bash
forge script script/DeployToken.s.sol --broadcast --rpc-url <YOUR_RPC_URL>
```

- After deployment, note down the contract address as it will be used for interactions and testing.

# Testing
- This project includes a suite of unit and integration tests to verify the ERC20 token's functionality.

```bash
forge test
```

and

```bash
forge coverage
```

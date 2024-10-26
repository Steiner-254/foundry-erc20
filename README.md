# ERC20 Token Project 🪙

![GitHub last commit](https://img.shields.io/github/last-commit/Steiner-254/foundry-erc20)
![GitHub issues](https://img.shields.io/github/issues/Steiner-254/foundry-erc20)
![GitHub license](https://img.shields.io/github/license/Steiner-254/foundry-erc20)

## Overview

Welcome to the **ERC20 Token Project**! This project provides a robust framework for creating and managing an ERC20 token on the Ethereum blockchain. Designed with developers in mind, this implementation offers straightforward, customizable token functionality for decentralized applications and tokenized ecosystems.

### Key Features:
- **ERC20 Standard Compliant**: Fully compatible with ERC20 standards, ensuring interoperability.
- **Mintable & Burnable**: Allows token minting and burning functionality, useful for dynamic supply management.
- **Automated Testing**: Built-in unit tests to verify all token functionalities.
- **Customizable Parameters**: Flexible token supply, name, and symbol settings.

## How it Works 🛠️

1. **Deploy the Token**: Initialize the contract with your desired token name, symbol, and initial supply.
2. **Mint & Burn**: Authorized accounts can mint new tokens or burn tokens from circulation.
3. **Token Transfers**: Tokens can be sent between accounts following standard ERC20 `transfer` and `approve` functions.
4. **Testing**: Comprehensive testing suite ensures all token functions operate as expected.

## Tech Stack ⚙️

- **Smart Contracts**: Written in Solidity, using the Foundry framework.
- **Testing Framework**: Forge for efficient, automated unit testing.
- **Deployment & Scripting**: Forge scripts for streamlined contract interactions.

## Directory Structure 📂

```bash
.
├── .github/workflows     # GitHub actions for CI/CD
├── lib                   # External libraries and dependencies
├── script                # Deployment and interaction scripts
├── src                   # Core smart contracts
│   └── ERC20.sol         # ERC20 token contract
├── test                  # Unit and integration tests
├── .gitignore            # Ignored files
├── README.md             # Project overview (this file)
├── foundry.toml          # Foundry configuration
├── Makefile              # Helper commands for build/test
```

## Local Setup 💻
- Clone the repository:

```bash
git clone https://github.com/Steiner-254/foundry-erc20.git
cd foundry-erc20
```

## Install Dependencies
- Ensure you have Foundry installed. If not, install it using:
```bash
curl -L https://foundry.paradigm.xyz | bash
foundryup
```

## Compile the Smart Contracts:
```bash
forge build
```

## Run Tests:
```bash
forge test
```

## Deploy to a Local Network:
- To deploy the contract locally or on a specified network, use the deployment script provided:

```bash
forge script script/DeployToken.s.sol --broadcast --rpc-url <YOUR_RPC_URL>
```

## License 📜
- This project is licensed under the MIT License. See the LICENSE file for details.

## Contributing 🤝
- Project Developed By: ![Steinet254](https://twitter.com/Steiner254)
- Feel free to fork this repo, submit issues, or create pull requests! Contributions are always welcome.

## Acknowledgments 🙌
- `Foundry` for providing an exceptional framework for Solidity development.
- `OpenZeppelin` for setting standards in secure contract implementations.
- `Ethereum Community` for supporting decentralized application development.
- `Cyfrin Updraft` for the learning content aiding to this project development.

## Happy Coding! 🚀

```vbet
Happy Web3 Revolution <3
```

# TokenBridgeX

TokenBridgeX is a cross-chain token bridging solution that facilitates secure and efficient transfers across EVM-compatible blockchains using Circle’s API, CCTP, and Polygon’s LxLy Bridge.

## Project Structure

The project is organized as follows:

- **contracts**: Contains smart contracts for token bridging functionality across different chains.
  - **cctp**: Contracts and interfaces for Circle's Cross-Chain Transfer Protocol (CCTP).
  - **LxLy**: Contracts and interfaces for bridging between Ethereum and Polygon zkEVM.
- **scripts**: Deployment scripts for deploying contracts to the blockchain.
- **test**: Contains test scripts for testing contract functionality and integration.
- **hardhat-config.ts**: Configuration for the Hardhat environment.

## Problem and Solution

### Problem
Cross-chain token transfers are often complex, expensive, and require navigating multiple platforms and protocols.

### Solution
TokenBridgeX provides a seamless and cost-effective solution for transferring tokens across major EVM-compatible chains, making cross-chain asset movement simpler and more accessible to DeFi users.

## Getting Started

### Prerequisites

1. **Node.js** (version 14 or above) - Ensure Node.js is installed on your machine.
2. **Hardhat** - This project uses Hardhat for contract development, testing, and deployment.

### Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/samarabdelhameed/TokenBridgeX-cir.git
cd TokenBridgeX-cir
npm install
```

## Project Structure

```plaintext
.
├── contracts            # Smart contracts
│   ├── cctp             # CCTP related contracts
│   ├── LxLy             # Polygon zkEVM bridge contracts
│   └── libraries        # Helper libraries for bridge functionality
├── scripts              # Deployment scripts
├── test                 # Tests for the contracts
├── hardhat.config.ts    # Hardhat configuration
├── package.json         # Project dependencies
└── README.md            # Project documentation
```

## Hardhat Setup and Commands

This project uses **Hardhat** to compile, deploy, and test smart contracts.

### Compile Contracts

Compile the smart contracts using the following command:

```bash
npx hardhat compile
```

### Run Tests

To test the contracts, execute:

```bash
npx hardhat test
```

Optionally, you can report gas usage while testing:

```bash
REPORT_GAS=true npx hardhat test
```

### Deployment

Deploy the contracts to a network of your choice. Use the provided deployment scripts in the `scripts` folder.

To deploy the contracts to a local Hardhat node:

1. Start a local node:

   ```bash
   npx hardhat node
   ```

2. Deploy the contracts:

   ```bash
   npx hardhat run scripts/deploy.ts --network localhost
   ```

For deployment to test networks (e.g., Rinkeby, Goerli):

1. Configure your `hardhat.config.ts` with network settings and API keys.
2. Deploy to the desired network:

   ```bash
   npx hardhat run scripts/deploy.ts --network <network-name>
   ```

### Verifying Contracts

Once deployed on a public testnet or mainnet, verify your contracts using:

```bash
npx hardhat verify --network <network-name> <contract-address> <constructor-arguments>
```

Replace `<network-name>`, `<contract-address>`, and `<constructor-arguments>` with your specific details.

## Supported Commands

```shell
npx hardhat help                   # List available Hardhat commands
npx hardhat compile                # Compile smart contracts
npx hardhat test                   # Run tests
npx hardhat node                   # Start local Hardhat network
npx hardhat run scripts/deploy.ts  # Deploy contracts
```

## Testing Structure

The `test` folder contains test files for each contract module:

- **cctp-bridge-arb.spec.ts**: Tests for Arbitrum bridging functionality via CCTP.
- **cctp-bridge-avax.spec.ts**: Tests for Avalanche bridging functionality via CCTP.
- **cctp-bridge-eth.spec.ts**: Tests for Ethereum bridging functionality via CCTP.
- **lxly-bridge-eth.spec.ts**: Tests for Ethereum bridging functionality via Polygon's LxLy Bridge.
- **lxly-bridge.spec.ts**: General tests for LxLy Bridge functionality.

These tests validate that each module works as expected across supported chains and ensures reliable cross-chain transfers.

## Important Files

- **hardhat-arb-fork.config.ts**: Configurations for Arbitrum fork testing.
- **hardhat-avax-fork.config.ts**: Configurations for Avalanche fork testing.
- **hardhat-eth-fork.config.ts**: Configurations for Ethereum fork testing.
- **supported-tokens.json**: JSON file listing supported tokens for bridging across chains.

## Future Enhancements
- **Multi-Routing**: Enable more flexible routing options for cross-chain transfers.
- **Expanded Token Support**: Additional tokens for bridging to improve compatibility.
- **Fiat On & Off-Ramp**: Feature to convert between crypto and fiat currencies.


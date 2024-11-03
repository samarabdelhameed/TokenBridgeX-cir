# TokenBridgeX

[![Website]()]()  
Effortlessly transfer tokens across multiple EVM-compatible blockchain networks.


## Overview

TokenBridgeX is being developed as a submission for the **Sigma Sprint: Global Multichain Builder Competition** under the **Circle Web3 Services Track**. The project aligns with the competition's focus on leveraging Circle's Web3 Services to create secure, composable, and scalable cross-chain infrastructure. By integrating with Circle’s APIs and smart contracts, TokenBridgeX aims to set a new standard for seamless token transfers across EVM-compatible chains.

![Flowchart](https://github.com/samarabdelhameed/pics/blob/main/flowchart%20my%20build%20.png)


## Key Features

- **Token Bridging Across EVM Chains:** Transfers of USDC, DAI, USDT, and WETH tokens are supported across chains.
- **Cost-Efficient Transactions:** Minimal fees with transparent caps for predictable transaction costs.
- **Expanding Token and Chain Support:** Built for scalability with upcoming multi-routing and fiat on/off-ramp features.

## Supported Chains and Tokens

| Chain              | Tokens                     |
|--------------------|----------------------------|
| Ethereum           | USDT, USDC, DAI, WETH      |
| Ethereum Goerli    | USDC                       |
| Arbitrum One       | USDT, USDC, DAI, WETH      |
| Arbitrum Goerli    | USDC                       |
| Avalanche          | USDT, USDC, DAI, WETH      |
| Avalanche Fuji     | USDC                       |
| Polygon PoS        | USDT, USDC, DAI, WETH      |
| Polygon Mumbai     | USDC                       |
| Polygon zkEVM      | USDC, USDT, DAI            |
| Polygon zkEVM Test | USDC                       |

## Transaction Fees

| Service           | Fee                          |
|-------------------|------------------------------|
| Circle API        | 4% (capped at $20)           |
| LxLy and CCTP     | 3% for stablecoins (capped at $20) |

## Future Enhancements

- **Multi-Routing:** Enhanced options for unrestricted token movement.
- **Expanded Token Support:** Addition of new tokens.
- **Fiat On & Off-Ramp:** Streamlined conversion between crypto and fiat.

## Smart Contract Integrations

### Circle CCTP (CrossChainBridge)

Enables seamless bridging of USDC across Ethereum, Arbitrum, and Avalanche networks.
- Ethereum Mainnet (Coming soon)
- Arbitrum Mainnet: `0x8e326D9F79a9D944C920fC7aE899Dd181ecB0491`
- Avalanche Mainnet: `0x8e326D9F79a9D944C920fC7aE899Dd181ecB0491`

### Polygon LxLy (RollupBridge)

Facilitates bridging of assets between Ethereum and Polygon zkEVM.
- Ethereum Mainnet (Coming soon)
- Polygon zkEVM Testnet: `0xA7e800f51dFb9Fd8C09067d7fC5757e06e57F27b`

## Technical Challenges Addressed

1. **Cross-Chain Asset Movement:** Supports seamless transactions across multiple chains using standardized APIs.
2. **Transaction Cost Reduction:** Affordable fees that are transparent and capped, making cross-chain interactions cost-effective.
3. **Liquidity and Router Issues on Testnets:** Optimized for stable token transfers, even on test networks, with smart contract deployment limited to testnet tokens (USDC).

## Folder Structure

```plaintext
.
├── backend       # Django backend for API and business logic
├── contracts     # Smart contracts for cross-chain functionality
└── frontend      # React application for user interface
```

## API Documentation



## Contributing

TokenBridgeX welcomes contributions in the form of bug reports, feature requests, and pull requests. Your participation helps in building a stronger, more robust cross-chain infrastructure.


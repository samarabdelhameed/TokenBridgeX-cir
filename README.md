# TokenBridgeX

[![Website]()]()  
Effortlessly transfer tokens across multiple EVM-compatible blockchain networks.


## Overview

TokenBridgeX is being developed as a submission for the **Sigma Sprint: Global Multichain Builder Competition** under the **Circle Web3 Services Track**. The project aligns with the competition's focus on leveraging Circle's Web3 Services to create secure, composable, and scalable cross-chain infrastructure. By integrating with Circle’s APIs and smart contracts, TokenBridgeX aims to set a new standard for seamless token transfers across EVM-compatible chains.

![Flowchart](https://github.com/samarabdelhameed/pics/blob/main/flowchart%20my%20build%20.png)

 Problem and Solution

#### Problem
In the rapidly evolving decentralized finance (DeFi) landscape, users frequently need to transfer tokens across multiple blockchains. However, this process is fraught with challenges:

1. **Fragmented Ecosystem**: Token liquidity is isolated on specific chains, creating a fragmented experience and forcing users to navigate different networks and platforms.
2. **Complexity of Cross-Chain Transfers**: Moving tokens across chains is a multi-step, complex process that requires technical knowledge and experience with multiple wallets and bridging protocols.
3. **High Transaction Fees**: Cross-chain transactions can incur significant fees, especially during periods of high network congestion, making frequent transfers costly.
4. **Limited Token and Chain Support**: Many existing solutions only support a limited number of tokens and blockchains, limiting flexibility and accessibility.
5. **Lack of Transparency in Fees**: Some platforms have hidden or unpredictable fees, leaving users uncertain about the total cost of transactions.

#### Solution
TokenBridgeX provides a streamlined, cost-effective, and user-friendly solution to cross-chain token transfers by integrating leading Web3 technologies like Circle's API, Circle CCTP, and Polygon's LxLy Bridge. Here’s how TokenBridgeX addresses the above challenges:

1. **Unified Cross-Chain Platform**: TokenBridgeX consolidates multiple blockchains, allowing users to transfer tokens across Ethereum, Polygon, Arbitrum, and Avalanche networks through a single, intuitive interface.
2. **Simplified User Experience**: The platform provides an easy-to-use interface for selecting tokens and target chains, with backend processes that automatically handle complex cross-chain interactions, eliminating the need for users to interact with multiple bridging protocols directly.
3. **Affordable and Predictable Fees**: TokenBridgeX uses a capped fee structure (e.g., Circle API: 4%, CCTP/LxLy: 3%), with clear and transparent pricing. This approach makes cross-chain transactions more affordable and predictable for users.
4. **Comprehensive Token and Chain Support**: TokenBridgeX supports major stablecoins (USDC, USDT, DAI, and WETH) across multiple chains and testnets, with plans for expanding token and chain compatibility to meet future needs.
5. **Transparent and Secure Transactions**: By integrating with well-known services like Circle and Polygon, TokenBridgeX provides secure transactions with transparent, upfront fee information, ensuring users are aware of transaction costs before initiating transfers.

Through these features, TokenBridgeX aims to empower DeFi users with a seamless, affordable, and secure solution for cross-chain asset movement, reducing the complexity of interacting with multiple blockchain networks.





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


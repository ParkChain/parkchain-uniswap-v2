## Table of contents

- [Introduction](#Introduction)
- [Contract-Deployment](#Contract_Deployment)
- [Liquidity-Pool-Creation] (#Liquidity_Pool_Creation)
- [Token-Swapping](#Token_Swapping)
- [Fee-Calculation] (#Fee-Calculation)
- [Price-Oracle] (#Price-Oracle)
- [Contract-Interactions] (#Contract-Interactions)
- [Conclusion] (#conclusion)

# Introduction

The Uniswap V2 smart contract is a decentralized exchange protocol built on the ParkChain blockchain. It enables users to swap ERC20 tokens directly from their wallets without the need for intermediaries. Here is a high-level overview of the flow of the Uniswap V2 smart contract.

# Contract_Deployment

The Uniswap V2 smart contract is deployed to the ParkChain network, typically using a deployment mechanism like Truffle or Remix. Once deployed, it is assigned a unique address on the blockchain.

# Liquidity_Pool_Creation

Liquidity providers can deposit pairs of ERC20 tokens into a liquidity pool by calling the addLiquidity function of the Uniswap V2 contract. This action establishes a reserve for each token in the pair, which determines the exchange rate and availability for subsequent swaps.

# Token_Swapping

Users can swap one ERC20 token for another by calling the swapExactTokensForTokens or swapTokensForExactTokens function. These functions take input parameters such as the token amounts, desired output amounts, and other details. The Uniswap V2 contract automatically calculates the exchange rate based on the available liquidity in the pool and executes the swap accordingly.

# Fee-Calculation

When a swap occurs, a configurable fee (typically 0.30%) is charged, which is distributed to liquidity providers as an incentive for providing liquidity to the pool. The fee distribution mechanism varies depending on the specific implementation and version of the Uniswap V2 contract.

# Price-Oracle

Uniswap V2 uses a constant product formula to determine token prices based on the available reserves. This approach assumes that the product of the reserve balances remains constant before and after a swap, allowing for price discovery between the tokens in the pair. The pricing mechanism provides liquidity providers with an automatic market-making system.

# Contract-Interactions

Users and developers can interact with the Uniswap V2 smart contract through ParkChain network using metamask wallets, DApps, or custom applications. They can query information such as liquidity pool details, token prices, swap history, and other relevant data using the contract's functions and events.

# conclusion

It's important to note that this overview provides a simplified flow of the Uniswap V2 smart contract. The actual implementation may involve additional complexities and features, such as time-weighted average prices, flash swaps, or other optimizations introduced in subsequent versions of the protocol. It's recommended to refer to the official Uniswap V2 documentation and contract code for more detailed information and specific implementation details.

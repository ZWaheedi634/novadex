# novadex
AMM DEX built on Robinhood Chain Testnet — Uniswap V2-style swap, liquidity pools &amp; LP tokens in a single Solidity file.
# NovaDEX ⚡

> A production-grade Automated Market Maker (AMM) 
> deployed on Robinhood Chain Testnet (Chain ID: 46630)

## Live Demo
🌐 [novadex.netlify.app](https://novasdex.netlify.app)

## Overview
NovaDEX is a fully on-chain decentralized exchange built 
from scratch using the Uniswap V2 constant product formula 
(x * y = k). It features a Factory/Router/Pair architecture, 
automatic LP token minting, a 0.3% swap fee, and a TWAP 
price oracle — all in a single deployable Solidity file.

## Live Contracts (Robinhood Testnet · Chain 46630)
| Contract           | Address    | Verified |
|--------------------|------------|----------|
| RobinhoodFactory   | 0x...      | ✅       |
| RobinhoodRouter    | 0x...      | ✅       |
| MockToken (WETH)   | 0x...      | ✅       |
| MockToken (USDC)   | 0x...      | ✅       |

## Architecture
```
RobinhoodFactory
└── creates → RobinhoodPair (LP token + AMM pool)

RobinhoodRouter (user entry point)
├── addLiquidity()
├── removeLiquidity()
├── swapExactTokensForTokens()
└── swapTokensForExactTokens()
```

## Features
- ♻️ Constant product AMM (x * y = k)
- 💧 Add & remove liquidity
- 🔁 Token swaps with 0.3% fee
- 🪙 Automatic LP token minting & burning
- 📈 TWAP price oracle (cumulative price tracking)
- 🏭 Factory pattern — unlimited trading pairs
- 🔒 Reentrancy protection on all state-changing functions
- ⛽ Gas optimized with uint112 packed reserves

## Tech Stack
| Layer        | Technology              |
|--------------|-------------------------|
| Smart Contract | Solidity 0.8.20       |
| Network      | Robinhood Chain Testnet |
| Frontend     | Ethers.js v6 + HTML/CSS |
| Hosting      | Netlify                 |
| Explorer     | Blockscout              |

## How to Use
1. Add Robinhood Testnet to MetaMask
```
Network Name → Robinhood Chain Testnet
RPC URL      → https://rpc.testnet.chain.robinhood.com
Chain ID     → 46630
Symbol       → ETH
Explorer     → https://explorer.testnet.chain.robinhood.com
```
2. Get test ETH from faucet
```
https://faucet.testnet.chain.robinhood.com
```
3. Visit the live demo → connect wallet → swap or add liquidity

## Local Development
No build tools needed. Just open index.html in browser.
```
git clone https://github.com/yourusername/novadex
cd novadex
open index.html
```

## License
MIT
```

---

## GitHub Profile Bio
```
Solidity Developer · Building DeFi on Robinhood Chain · 
AMM · DEX · Smart Contracts
```

---

## Netlify Site Description
```
NovaDEX — Decentralized Exchange on Robinhood Chain Testnet
```

---

## Twitter/X Bio (if you post about it)
```
Just deployed a full Uniswap V2-style AMM DEX on 
Robinhood Chain Testnet from scratch.

Factory + Router + Pair architecture
0.3% swap fee
LP token minting
TWAP oracle
Single Solidity file

Live → novadex.netlify.app
Code → github.com/you/novadex

#Robinhood #DeFi #Solidity #Web3

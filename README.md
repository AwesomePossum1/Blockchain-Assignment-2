# On-Chain Story Relay dApp

A decentralized, collaborative storytelling application built on Ethereum. Anyone can add a line to the story, but with a twist: **you cannot write two lines in a row**, ensuring a communal relay experience. Once the story reaches 10 lines, any user can trigger a chapter reset.

## Smart Contract Details
* **Contract Name:** `OnChainStory`
* **Network:** Sepolia Testnet
* **Deployed Contract Address:** `0x16B5a9EfbB74D3883d369b96d474085Af29e46d6`

---

## Features
* **Decentralized Storage:** All sentences are permanently stored and concatenated on the blockchain.
* **Turn-Based Rule Enforcement:** Smart contract logic prevents spamming by blocking consecutive submissions from the same wallet.
* **MetaMask Integration:** Connects seamlessly using Ethers.js v6 for read and write transactions.
* **Responsive Web Interface:** Single-page HTML/CSS UI styled with modern cards and real-time transaction logs.

---

## Setup & Installation

### Prerequisites
* [MetaMask](https://metamask.io/) browser extension installed and configured with Sepolia testnet ETH.
* [XAMPP](https://www.apachefriends.org/) (or any local web server like VS Code Live Server).

### Local Running Instructions
1. Clone or download this repository into your local server directory (e.g., `C:\xampp\htdocs\story-dapp\`).
2. Ensure your `index.html` references the correct deployed contract address:
   ```javascript
   window.CONTRACT_ADDR = '0x16B5a9EfbB74D3883d369b96d474085Af29e46d6';

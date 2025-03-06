# 0g-Labs-Testnet

A bot for automated token swapping on 0G-Newton-Testnet with multi-wallet support.

> Faucet: https://hub.0g.ai/faucet
> 
> Swap: https://hub.0g.ai/swap
> 
> Upload File: https://storagescan-newton.0g.ai/tool
> 
# Features

- ✅ Support for multiple private keys/wallets

- 🔄 Random token swapping based on available liquidity pools

- ⏱️ Configurable transaction count and timing

- 👨‍💻 User-friendly interface for wallet selection

- 📊 Detailed logging of swap activities

## Setup

1. Clone the repository
```bash
git clone https://github.com/chichiops/0g-Labs-Testnet.git
cd 0g-Labs-Testnet
```
2. Install dependencies
```bash
npm install
```
3. Configure your .env file with private keys:
```bash
# Option 1: Single wallet
WALLET_PRIVATE_KEY=your_private_key_here

# Option 2: Multiple wallets
WALLET_PRIVATE_KEY_1=your_first_private_key_here
WALLET_PRIVATE_KEY_2=your_second_private_key_here
WALLET_PRIVATE_KEY_3=your_third_private_key_here

# Bot configuration
SWAP_DELAY=60
MIN_BALANCE_FOR_SWAP=0.1
```
4. Run the bot with:
```bash
node index.js
```

**Notes**

- The bot will automatically distribute transactions over the specified time period

- If no time period is specified, random delays between 30s and 5min will be used

- The bot requires a minimum token balance (configurable in .env) to perform swaps

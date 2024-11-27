

# 🌊💸 Raydium Buy-Sell Bot 💹🚀

A **Solana-based bot** that automates **buying and selling tokens** on Raydium liquidity pools. Leverage the power of the blockchain for seamless trading and liquidity interactions! 🌟✨

---

## ✨ Features

✔️ **Automated Transactions**: Performs **buy-and-sell** operations for any token with ease.  
✔️ **Dynamic Pool Handling**: Automatically fetches pool information and derives keys.  
✔️ **Slippage Protection**: Ensures optimal trades with slippage management.  
✔️ **Smart Wallet Handling**: Creates token accounts only if necessary.  

---

## 🛠️ Prerequisites

Before running the bot, make sure you have the following in place:  

1️⃣ **Node.js**: Install [Node.js](https://nodejs.org/). 🖥️  
2️⃣ **Solana CLI**: Set up and configure the Solana CLI. 🛠️  
3️⃣ **Environment Variables**:  
   - `MAIN_KP`: 🗝️ Your wallet's private key in Base58 format.  
   - `RPC_URL`: 🌐 A reliable Solana RPC endpoint URL.  

---

## 📦 Installation

1️⃣ **Clone the Repository**:  
   ```bash
   git clone <repository-url>
   cd <repository-name>
   ```  

2️⃣ **Install Dependencies**:  
   ```bash
   npm install
   ```  

3️⃣ **Set Environment Variables**:  
   Create a `.env` file with the following:  
   ```
   MAIN_KP=<your-base58-private-key>
   RPC_URL=<your-rpc-url>
   ```  

4️⃣ **Update the Token**:  
   Replace `baseMintStr` with your target token’s mint address. 🪙  

---

## 🚀 Usage

1️⃣ **Start the Bot**:  
   ```bash
   npm start
   ```  

2️⃣ **What Happens**:  
   - 🧮 Fetches token and pool details.  
   - 🔄 Executes **buy** and **sell** transactions.  
   - 📊 Logs the **transaction details** and provides a **Solana transaction link**.  

3️⃣ **Example Log Output**:  
   ```
   Main wallet: <your-public-key>  
   Wallet balance: 2.345 SOL  
   Derived Pool Keys: ...  
   Buy Transaction Amount: 0.0001 SOL  
   Sell Transaction Amount: 0.0001 SOL  
   Transaction Link: https://solscan.io/tx/<transaction-id>
   ```  

---

## 🌟 Key Components

### ⚙️ `buySellToken(token: PublicKey)`
Handles the entire process:  
- 🔍 Fetches and caches essential data (pool keys, token decimals, etc.).  
- 💹 Computes the optimal **input/output amounts** for trading.  
- ✍️ Creates and signs transactions for **buy and sell operations**.  

### 🚦 `run()`
- 🖋️ Logs the wallet address and current balance.  
- 🔄 Invokes `buySellToken()` for the specified token.  

---

## 📚 Example Configuration

- **Token Mint**: `6LRHCKvqCX9JuQj8Fkx8yEM3c1PpyrV9NuPujc9Qpump` 🪙  
- **Liquidity Pool**: `HRUsdnW2B49DQS64UoPJjcciRHSi3sBSBfnDmdEEzCRN` 🌊  
- **Slippage**: 1%  

---

## 📎 Links

- 🌐 [Raydium Docs](https://raydium.gitbook.io/)  
- 🛠️ [Solana Web3.js](https://solana-labs.github.io/solana-web3.js/)  
- 💻 [Node.js](https://nodejs.org/)  

---

Feel free to ❤️ fork, ⭐ star, or 🛠️ contribute to this project! 🚀

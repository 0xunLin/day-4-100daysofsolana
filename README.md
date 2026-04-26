# Day 4: Solana Wallet Connect

A simple, modern web application that demonstrates how to connect to Solana wallets using the Wallet Standard and fetch account balances using the new Solana Web3.js v2 (`@solana/kit`).

## 🚀 Functions

- **Wallet Discovery**: Automatically detects compatible Solana wallets (like Phantom, Solflare, etc.) installed in the browser.
- **Dynamic Wallet List**: Displays a list of available wallets with their icons and names.
- **Secure Connection**: Facilitates a secure connection request to the user's selected wallet.
- **Real-time Balance Fetching**: Uses the Solana Devnet RPC to fetch and display the SOL balance of the connected account.
- **Account Abstraction Ready**: Built using modern standards for better compatibility.
- **Disconnect Flow**: Allows users to safely disconnect their wallet from the application.

## 🧠 Learnings

During this project, I explored:
- **Solana Web3.js v2 (`@solana/kit`)**: Transitioning from the legacy library to the new, more modular and lightweight kit. Specifically using `createSolanaRpc` and `devnet` helpers.
- **Wallet Standard (`@wallet-standard/app`)**: Understanding how to interact with browser-based wallets in a unified way without needing wallet-specific adapters.
- **Asynchronous RPC Calls**: Managing promises for balance fetching and error handling for connection rejections.
- **Dynamic DOM Manipulation**: Building a responsive UI that updates its state based on wallet events (registration, connection, disconnection).
- **Lamport Conversion**: Handling large numbers and converting lamports to a human-readable SOL format.

## 🛠️ Setup Instructions

Follow these steps to run the project locally:

### 1. Prerequisites
- **Node.js** (v18 or higher recommended)
- **A Solana Wallet Extension** (e.g., [Phantom](https://phantom.app/)) installed in your browser.

### 2. Installation
Clone the repository and navigate to the project directory:
```bash
cd day-4-wallet
npm install
```

### 3. Running the Development Server
Start the Vite development server:
```bash
npm run dev
```
Open the provided local URL (usually `http://localhost:5173`) in your browser.

### 4. Usage
1. Ensure your wallet is set to **Devnet**.
2. Click on your wallet provider in the list.
3. Approve the connection request.
4. View your balance!

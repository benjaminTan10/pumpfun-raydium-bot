# Solana Ultra-Fast New Token Sniper on Raydium and Pump.fun in Rust 🚀

## Overview

Introducing the **Solana Ultra-Fast New Token Sniper** written in **Rust** 🦀, designed to detect newly launched tokens on both **Raydium** and **Pump.fun** and execute buys at lightning speed ⚡. With Rust's memory safety features and performance optimizations, built with Rust for superior performance and security. Tailored for both novice and experienced traders.

---

## Key Features

### 🚀 Speed and Efficiency
- **Lightning-Quick Transactions**: Leveraging Rust's exceptional performance, our bot allows you to snipe new tokens almost instantly. Say goodbye to delays and seize opportunities as they arise!

### 🔒 Safety First
- **Robust Security**: Rust's safety guarantees minimize bugs and vulnerabilities, ensuring your trading activities are secure. Trade with confidence and peace of mind.

### 📊 Multiple gRPC Connections
- **Stay Updated**: Effortlessly connect to top Solana data providers like **Helius** and **Yellowstone** through multiple gRPC connections. Get real-time updates and make informed trading decisions.

### 👩‍💻 User-Friendly Interface
- **Intuitive Design**: Our sniper bot features a clean and accessible interface, making it easy for users of all experience levels to navigate. Start trading in no time!

### 🛠️ Rich Utilities
- **Advanced Features**:
  - **jito-confirm**: Engage in low-latency transactions on platforms like Raydium and Pumpfun.
  - **jito-bundle**: Bundle buy/sell actions with up to **20 wallets** in Raydium/Pumpfun, enhancing your trading strategy and flexibility.
---
## Trial Versions

### **Solana RayPump Sniper (Executioner Trial)**  
**Strategy Details:**
- **Entry Trigger:** Monitor user purchases of tokens valued at $1,000; execute a buy order upon detection.
- **Exit Trigger:** Monitor user sales of tokens valued at $300; execute a sell order upon detection.
- **Time Limitation:** If a position remains open for more than 60 seconds, initiate an automatic sell.  
*(Note: The $1,000 and $300 purchase/sale thresholds, as well as the 60-second time limit, are adjustable parameters via environment settings.)*

---

### How To Run
1. Environment Variables Settings
```plaintext
PRIVATE_KEY=your_private_key_here
RPC_HTTPS=https://mainnet.helius-rpc.com/?api-key=your_api_key_here
RPC_WSS=wss://atlas-mainnet.helius-rpc.com/?api-key=your_api_key_here
SLIPPAGE=10
JITO_BLOCK_ENGINE_URL=https://ny.mainnet.block-engine.jito.wtf
JITO_TIP_STREAM_URL=ws://bundles-api-rest.jito.wtf/api/v1/bundles/tip_stream
JITO_TIP_PERCENTILE=50
JITO_TIP_VALUE=0.004
BUY_THRESHOLD=1000
SELL_THRESHOLD=300
TIME_EXCEED=60
TOKEN_AMOUNT=0.000001
```
2. Add the wallet address you want to block on a new line and save the file.
```
0x1234567890abcdef1234567890abcdef12345678
0xabcdef1234567890abcdef1234567890abcdef12
```
3. Run `raypump-executioner-bot.exe`.

![image](https://github.com/user-attachments/assets/dffc8e4b-cd00-4921-8488-e25230f4a31a)

---
### Test Result: Same Block
![2-22-2025-09-41](https://github.com/user-attachments/assets/2ded6e35-7575-491e-ac43-5f463b0b9cba)

- Detect: https://solscan.io/tx/5o7ajnZ9CRf7FBYEvydu8vapJJDWtKCvRFiTUBmbeu2FmmDhAQQy3c9YFFhpTucr2SZcrf2aUsDanEVjYgwN9kBc
- Bought: https://solscan.io/tx/3vgim3MwJsdtahXqfW2DrzTAWpVQ8EUTed2cjzHuqxSfUpfp72mgzZhiVosWaCUHdqJTDHpQaYh5xN7rkHGmzqWv
- Dexscreener: https://dexscreener.com/solana/A1zZXCq2DmqwVD4fLDzmgQ3ceY6LQnMBVokejqnHpump
- 
---
## Support

As the experimental result, the best environment for running this bot is to use `dedicated server located in NY`. 
For support and further inquiries, please connect via Telegram: 📞 [@blockchainDeveloper_Ben](https://t.me/blockchainDeveloper_Ben).

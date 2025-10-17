# 🎰 SpinToWin — Farcaster MiniApp on Base

**SpinToWin** is an interactive **Farcaster MiniApp (Frame)** that lets users spin a wheel and earn **SuperInu ($SUPINU)** rewards directly on **Base Mainnet**.

---

## 🌐 Live Demo
**MiniApp URL:**  
👉 [https://spintowin.vercel.app/](https://spintowin.vercel.app/)

**Farcaster Post Example:**  
🎯 Spin the wheel and win $SUPINU rewards on Base!
https://spintowin.vercel.app/

yaml
Copy code

---

## 🧩 Features
- 🎡 Interactive spin wheel with 8 reward segments  
- 💰 Real $SUPINU rewards on Base mainnet  
- 🪙 Randomized reward values ($0.01 – $0.05)  
- 🔐 Smart contract verified on BaseScan  
- 🧠 Fully compatible with Farcaster MiniApp SDK  
- ⚡ Deployed via GitHub + Vercel for instant frame loading  

---

## 🪙 Smart Contract
**Contract Name:** `BaseSpinGame`  
**Network:** Base Mainnet  
**Token Used:** [SuperInu ($SUPINU)](https://basescan.org/token/0x063eDA1b84ceaF79b8cC4a41658b449e8E1F9Eeb)

**Contract Address:**  
0x727D4DB40aEfD9F213564F710A96318b9da8dBDB

makefile
Copy code

**Owner:**  
0x0A3FE49B6bD9a461B7Fe957EDC3761c3b1a255b1

yaml
Copy code

---

## ⚙️ Tech Stack
| Layer | Technology |
|-------|-------------|
| Frontend | HTML + JavaScript |
| Web3 SDK | [Wagmi](https://wagmi.sh/) + [Farcaster MiniApp SDK](https://docs.farcaster.xyz/) |
| Chain | [Base Mainnet](https://base.org) |
| Token | SuperInu ($SUPINU) |
| Hosting | [Vercel](https://vercel.com) |
| Source Control | GitHub |

---

## 🧠 How It Works

1. **User Launches Frame**  
   - Via Warpcast post or link.  
2. **Connects Wallet (via Farcaster SDK)**  
   - Farcaster MiniApp auto-connects to wallet.  
3. **Spins the Wheel**  
   - Randomly selects 1 of 8 reward segments.  
4. **Reward Assigned**  
   - Smart contract logs `SpinResult` event.  
5. **User Withdraws**  
   - User calls `withdraw()` → receives $SUPINU token directly.

---

## 🏗️ Local Setup

### 1️⃣ Clone the Repo
```bash
git clone https://github.com/<your-username>/spintowin.git
cd spintowin
2️⃣ Install Dependencies
This MiniApp uses no npm build system — just HTML + JS.
If you want to extend it with Next.js:

bash
Copy code
npm install
3️⃣ Folder Structure
pgsql
Copy code
/public
├── index.html
├── image.png
├── splash.png
├── icon.png
├── baseClaim.json
└── .well-known/
    └── farcaster.json

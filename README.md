# 🚀 DAC Node Setup Script (VPS / WSL)

### by CryptoDropScout

Run a DAC Chain Testnet node with wallet creation + faucet flow + background execution — all in one script.

---

## ⚡ Features

* 🔐 Auto wallet creation (keystore)
* 💧 Faucet-ready workflow
* 🚀 One-command node setup
* 🖥️ Runs in background using `screen`
* 🌐 Works on VPS & WSL
* 🧹 Clean setup (no Docker needed)

---

## 🧠 Requirements

* Ubuntu VPS / WSL (20.04 / 22.04 / 24.04)
* Internet connection
* Basic terminal usage

---

## 📥 Installation

👇 Copy & run:

```bash
wget https://raw.githubusercontent.com/Hunterkak/dac-node-cryptodropscout/main/dac.sh && chmod +x dac.sh && ./dac.sh
```

---

## 🔐 Wallet Setup

The script will:

* Create a new wallet using DAC CLI
* Ask you to set a password
* Store keystore file locally

📁 Wallet location:

```bash
~/dac-node/data/keystore
```

⚠️ IMPORTANT:

* Save your password
* Backup keystore file
* No recovery if lost

---

## 💧 Faucet Step

After wallet creation:

* Copy your wallet address
* Send faucet (DAC testnet tokens)
* Confirm inside script

---

## 🚀 Node Execution

Node runs automatically in background using:

```bash
screen
```

---

## 📜 View Logs

```bash
screen -r dacnode
```

Detach safely:

```bash
CTRL + A + D
```

---

## 🛑 Stop Node

```bash
screen -S dacnode -X quit
```

---

## 🧹 Cleanup (Full Reset)

```bash
wget https://raw.githubusercontent.com/Hunterkak/dac-node-cryptodropscout/main/cleanup.sh && chmod +x cleanup.sh && ./cleanup.sh
```

---

## 🧠 Node Types (DAC Network)

* Light Node → basic participation
* Validator → requires ~1000 DACT
* Supervisor → requires ~100,000 DACT

👉 This script runs a **Testnet node**

---

## 🔒 Security Tips

* Never share private key
* Backup keystore file offline
* Use strong password

---

## ⚡ Notes

* Uses official DAC binary
* No Docker required
* Works on most VPS providers
* Compatible with WSL

---

## 👑 Author

**CryptoDropScout 🚀**

---

## ⭐ Support

If this helped you:

* ⭐ Star the repo
* 🔁 Share with others
* 🔥 Run nodes like a pro

📢 X (Twitter): **@cryptodrpscout**

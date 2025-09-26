# 🚀 **Termux Bot Setup Guide**  

Welcome to the **Termux Bot Setup Guide**! This guide will help you install and run the bot on your mobile device using **Termux**. Please follow each step carefully.  

> ⚠️ **Disclaimer:**  
> - This bot is intended for educational and personal use only.  
> - The developer is **not responsible** for any misuse or consequences of running this bot.  
> - Using automation tools may violate the terms of service of some platforms—use it at your own risk.  

---

## 📌 **Table of Contents**  

1. [📋 Prerequisites](#-prerequisites)  
2. [📥 Installing the Bot](#-installing-the-bot)  
3. [⚙️ Configuring the Bot](#-configuring-the-bot)  
4. [▶️ Running the Bot](#-running-the-bot)  
5. [🔄 Updating the Bot](#-updating-the-bot)  
6. [📞 Contact & Support](#-contact--support)  

---

## 📋 **Prerequisites**  

Before installing the bot, ensure you have the following installed on Termux:  

✅ **Termux App:** [Download Here](https://t.me/KeoAirDropFreeNe/257/32384)  
✅ **Node.js (v22.11.0)**  
✅ **npm (v10.9.0)**  

### **🛠 Initial Termux Setup**  
Open Termux and run the following commands to update and install dependencies:  

```bash
pkg update && pkg upgrade -y
termux-setup-storage
pkg install nodejs-lts git -y
```

Verify installation:  
```bash
node -v
npm -v
```

---

## 📥 **Installing the Bot**  

### **🔹 Method 1: Install via Git (Recommended)**  

1️⃣ **Clone the bot repository:**  
```bash
git clone <repository-url> 
cd bot-folder
```

2️⃣ **Install dependencies:**  
```bash
npm install --force -g user-agents axios meo-forkcy-proxy meo-forkcy-utils meo-forkcy-logger meo-forkcy-colors ethers
```

---

### **🔹 Method 2: Manual Installation**  

1️⃣ **Download the bot files manually** and extract them into a folder.  
2️⃣ **Navigate to the folder and install dependencies:**  
```bash
cd /path/to/bot-folder
npm install --force
```

---

## ⚙️ **Configuring the Bot**  

Before running the bot, make sure you have the necessary configuration files set up.  

### **1️⃣ `configs.json` - Main Configuration**  
Modify this file to adjust bot settings:  
```json
{}
```

### **2️⃣ `datas.txt` - User Data File**  
```txt
abc...xyz
abc...xyz
abc...xyz
```

### **3️⃣ `wallets.txt` - Wallet Addresses**  
```txt
0xabc...xyz
0x123...def
0x789...ghi
```

### **4️⃣ `proxies.txt` - Proxy List (Optional)**  
```txt
http://host:port
https://host:port
socks4://host:port
socks5://host:port
http://user:password@host:port
https://user:password@host:port
socks4://user:password@host:port
socks5://user:password@host:port
```

---

## ▶️ **Running the Bot**  

### **Run the bot normally:**  
```bash
node meomundep.js
```

If you encounter permission issues:  
```bash
chmod +x meomundep.js
```

### **Run the bot in the background (Optional)**  

To prevent the bot from stopping when you close Termux:  

✅ **Using `nohup` (Logs saved to `output.log`)**  
```bash
nohup node meomundep.js > output.log 2>&1 &
```

✅ **Using `tmux` (If installed)**  
```bash
tmux new-session -d -s bot_session 'node meomundep.js'
```

✅ **Check running processes:**  
```bash
ps aux | grep node
```

✅ **Stop the bot manually:**  
```bash
killall node
```

---

## 🔄 **Updating the Bot**  

### **🔹 If Installed via Git:**  
```bash
cd bot-folder
git pull
npm install
```

### **🔹 If Installed Manually:**  
Download the updated version and replace your old files.  

---

## 📞 **Contact & Support**  

📞 [Contact for work or order scripts](https://t.me/MeoMunDep)
💸 [Support me via Donate](https://t.me/KeoAirDropFreeNe/312/27801)
⚡ [Boost-Channel](https://t.me/boost/KeoAirDropFreeNee)

🌐 [Script Group](https://t.me/keoairdropfreene) | [Chat Group](https://t.me/keoairdropfreeneee) | [TikTok](https://www.tiktok.com/@meomundep) | [Instagram](https://www.instagram.com/meomundep) | [YouTube Channel](https://www.youtube.com/@keoairdropfreene)

---

__Use this script at your own risk and do not sell or try to modify it.__
  
🚀 **Enjoy using the bot on Termux!** 🚀

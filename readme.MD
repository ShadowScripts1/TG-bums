# TG-bums Bot

AUTO CLAIM FOR BUMS / [@bums](https://t.me/bums/app?startapp=ref_T5P4EMOc)

[![Join our Telegram](https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/shadowscripters)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ShadowScripts1)

---

# Table of Contents
- [Warning](#warning)
- [Available Features](#available-features)
- [Getting Started](#getting-started)
- [Configuration Files](#configuration-files)
- [Usage](#usage)
- [Viewing Reports](#viewing-reports)
- [Error Table](#error-table)
- [Support Me](#support-me)
- [Contact](#contact)
- [Thank You](#thank-you)

---

## Warning

> **All risks are borne by the user.** 

---

## Available Features

- [x] Automatic Claim Every 8 Hours
- [x] Automatic Daily Check-In (Login)
- [x] Automatic Claim of Referral Results
- [x] Proxy Support
- [x] Automatic Task Completion
- [x] Automatic Game Play after Claiming
- [x] Multi-process Support
- [x] Random User-Agent
- [x] Total Balance Report of All Accounts
- [x] Waiting Time Before Starting the Program

---

## 🚀 Getting Started

Follow these steps to set up and run the bot:

### 1. Clone the Repository

Clone the repository from GitHub:

```bash
git clone https://github.com/ShadowScripts1/TG-bums.git
```

### 2. Navigate to the Bot Directory

After cloning, navigate to the bot’s directory:

```bash
cd TG-bums
```

### 3. Install NodeJS and Required Dependencies

- Download and install [NodeJS](https://nodejs.org/).
- Then, install the necessary modules for the bot:

```bash
npm i user-agents cloudscraper axios colors p-limit https-proxy-agent socks-proxy-agent
```

### 4. Prepare Configuration Files

To ensure the bot runs properly, set up the following configuration files in the `TG-bums` directory:

#### `configs.json` - Main Configuration

Create a `configs.json` file with the following settings:

```json
{
  "maxCardPrice": 1000000000,
  "howManyEnergyUpgrade": 1,
  "howManyRecoveryUpgrade": 1,
  "howManyTapUpgrade": 1,
  "howManyBonusChanceUpgrade": 1,
  "howManyBonusRatioUpgrade": 1,
  "combo": "101,102,103", // refer to comboList.json to find today's combo
  "limit": 5, // number of accounts to run in a row
  "countdown": 300, // time to restart all accounts in seconds
  "country_time": "vi-VN" // timestamp based on the country
}
```

#### `datas.txt` - User Data

In `datas.txt`, add query data with each account on a new line:

```txt
query_id.../user...
query_id.../user...
query_id.../user...
```

#### `wallets.txt` - Wallet Addresses

Add wallet addresses as needed, with each address on a new line:

```txt
abc...xyz
abc...xyz
abc...xyz
```

#### `proxies.txt` - Proxy Configuration (Optional)

If you have proxy information, add it here. Leave blank if you don’t have one. Format examples:

```txt
http://user:password@host:port
https://user:password@host:port
socks4://user:password@host:port
socks5://user:password@host:port
```

---

## 💡 Usage

1. After setting up, navigate to the bot directory if you haven’t already:

   ```bash
   cd TG-bums
   ```

2. Start the bot with the following command:

   ```bash
   node bot.js
   ```

🎇 **Enjoy the bot!**

---

## Viewing Reports

To view a report of the total balance of all accounts, run:

```bash
node report.js
```

---

## Error Table

| Error                 | Description                                      |
| --------------------- | ------------------------------------------------ |
| failed get json error | Server response not in JSON. Check http.log.     |
| failed get task list  | Missing server response. Check http.log.         |
| cannot start game     | Server issue. Check http.log.                    |

---

## 💱 Support Me

If you found this tool useful, consider supporting:

- **EVM**: `0x7BeE9994a631523e22A3aB83039c196bFc6BC513`
- **SOLANA**: `6mbFy6AojWo3J5ksa1SYHHyCWw5Bms4p9McKmaFkCsyW`

---

## Contact

For questions or support, contact [Scripters Enclave chat](https://t.me/chatwithscripters).

---

## Thank You


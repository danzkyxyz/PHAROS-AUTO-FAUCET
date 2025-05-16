# Pharos Auto Faucet
Pharos Auto Faucet is a Python-based automation script designed to streamline the process of claiming testnet tokens from the Pharos Testnet faucet, performing daily check-ins, and transferring PHRS balances to a main wallet. Tailored for developers and testers on the Pharos Testnet, this tool supports multiple wallets, proxy rotation for anonymity, and a rich console interface with color-coded logs and tables for enhanced user experience. It includes robust error handling to ensure reliable operation across various network conditions.

## 🚀 Key Features
✨ Multi-Wallet Support: Processes multiple wallets from pvkey.txt for faucet claims and check-ins.
✨ Daily Check-In Automation: Automatically performs daily check-ins to earn additional rewards.
✨ PHRS Balance Transfer: Transfers all PHRS balances to a main wallet specified in receiver.txt.
✨ Proxy Rotation: Rotates proxies from proxy.txt to prevent IP-based restrictions.
✨ Rich Console UI: Displays progress with vibrant tables, panels, and emojis using the rich library.
✨ Robust Error Handling: Includes retry mechanisms and detailed logging for failed operations.
✨ Configurable File Inputs: Supports custom private key, proxy, and receiver address files.
🛠️ Use Case
This script is ideal for developers and testers who need to claim PHRS testnet tokens, perform daily check-ins, and consolidate balances for testing smart contracts, dApps, or other blockchain projects on the Pharos Testnet. It eliminates manual interactions with the faucet and check-in system, saving time and ensuring efficient token management across multiple wallets.

## Requirements
⚙️ Python 3.8+
⚙️ Required libraries: web3, eth-account, requests, fake-useragent, rich
⚙️ List of private keys (pvkey.txt)
⚙️ Main wallet address (receiver.txt)
⚙️ Proxy list (proxy.txt, optional)
📦 Installation

## Clone the repository:

```bash
git clone https://github.com/yourusername/pharos-auto-faucet.git
cd pharos-auto-faucet
```

Install dependencies:

```bash
pip install web3 eth-account requests fake-useragent rich
```

## Configure the script:
- Prepare pvkey.txt with private keys (one per line, without 0x prefix).
- Add the main wallet address to receiver.txt (single Ethereum address, with or without 0x).
- Optionally, add proxies to proxy.txt (format: http://user:pass@host:port).
- I recommend using proxies from DATAIMPULSE for affordable and budget-friendly prices (just $5 for 5GB proxy data).

## Run the script:

```bash
python main.py
```

or

```bash
python3 main.py
```

## The script will:
- Load private keys, receiver address, and proxies.
- Claim PHRS tokens from the Pharos Testnet faucet for each wallet.
- Perform daily check-ins for additional rewards.
- Transfer all PHRS balances to the main wallet specified in receiver.txt.
- Display progress with a rich console interface, including tables and color-coded logs.


## Configuration

Edit the following variables in the script to customize behavior:

NETWORK_CONFIG: Network details (e.g., RPC URL, chain ID).
pvkey.txt: List of private keys for wallets.
receiver.txt: Main wallet address for PHRS transfers.
proxy.txt: List of proxies for rotation (optional).

## 📝 Notes
- Ensure pvkey.txt contains valid private keys without 0x prefixes.
- Verify the receiver address in receiver.txt is correct to prevent loss of funds.
- Proxies are recommended to avoid faucet rate limits, but the script works in direct mode if proxy.txt is absent.
- The script assumes a stable internet connection for Web3 and API interactions.
- Always back up private keys and test the script with small amounts first.

## Join Our Community 🌐
For updates, support, or to share feedback, join our Telegram channel:

```bash
https://t.me/airdropdxns
```

## Buy Me a Coffee ☕
If you find this script helpful and want to support its development, consider sending a small donation to the following EVM wallet address:

```bash
0xd111dbc26d6ad2df49e4ed06044958dff2c3feda
```

Your support is greatly appreciated and helps keep the project maintained!

## Disclaimer ⚠️
This tool is for educational and testing purposes only. Use it responsibly and in accordance with the Pharos Testnet faucet's terms of service. The author is not responsible for any misuse or issues arising from the script's use. Always verify wallet addresses and private keys to prevent loss of funds.

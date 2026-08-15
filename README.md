# SAYMAN CLI

Official Command Line Interface for the **SAYMAN Blockchain**.

Manage wallets, send transactions, stake tokens, deploy smart contracts, and interact with the SAYMAN network directly from your terminal.

---

## Features

* Create and manage wallets
* Check wallet balances
* Send SAYN tokens
* Stake & unstake tokens
* Deploy JavaScript smart contracts
* Call smart contract methods
* View validator information
* Configure custom RPC endpoints
* Lightweight and easy to use

---

# Installation

## Global Installation (Recommended)

```bash
npm install -g @sayman/cli
```

Verify the installation:

```bash
sayman --version
```

or

```bash
sayman --help
```

---

# Configure RPC Endpoint

By default the CLI uses the official SAYMAN Public Testnet.

To use another node:

```bash
sayman config https://your-node.com/api
```

---

# Wallet Commands

## Create Wallet

```bash
sayman wallet create
```

Example Output

```
Address:
0x1234...

Private Key:
xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
```

---

## Import Wallet

```bash
sayman wallet import
```

---

# Account Commands

## Check Balance

```bash
sayman balance YOUR_ADDRESS
```

Example

```bash
sayman balance 0x381759097c41959499de2496ab522f11016faa9b
```

---

# Network

View current network information.

```bash
sayman network
```

---

# Send Tokens

```bash
sayman send RECEIVER_ADDRESS AMOUNT --privateKey YOUR_PRIVATE_KEY
```

Example

```bash
sayman send 0xabc123... 100 --privateKey YOUR_PRIVATE_KEY
```

---

# Stake Tokens

```bash
sayman stake 100 --privateKey YOUR_PRIVATE_KEY
```

---

# Unstake Tokens

```bash
sayman unstake 50 --privateKey YOUR_PRIVATE_KEY
```

---

# Validators

List all validators.

```bash
sayman validators
```

---

# Deploy Smart Contract

```bash
sayman deploy contract.js --privateKey YOUR_PRIVATE_KEY
```

---

# Call Smart Contract

```bash
sayman call CONTRACT_ADDRESS METHOD_NAME
```

Example

```bash
sayman call 0xabc123... balanceOf '["0x123..."]'
```

---

# Help

Display all available commands.

```bash
sayman --help
```

Help for a specific command:

```bash
sayman wallet --help
```

---

# Available Commands

| Command      | Description            |
| ------------ | ---------------------- |
| `wallet`     | Wallet management      |
| `config`     | Configure RPC endpoint |
| `network`    | Network information    |
| `balance`    | Check wallet balance   |
| `send`       | Send SAYN tokens       |
| `stake`      | Stake SAYN             |
| `unstake`    | Unstake SAYN           |
| `validators` | List validators        |
| `deploy`     | Deploy smart contract  |
| `call`       | Call smart contract    |

---

# Updating

Update to the latest version.

```bash
npm update -g @sayman/cli
```

---

# Uninstall

```bash
npm uninstall -g @sayman/cli
```

---

# Documentation

Official Documentation

https://sayman-docs.vercel.app

---

# Public Testnet

RPC Endpoint

```
https://sayman.onrender.com/api
```

Explorer

```
https://sayman.onrender.com
```

Faucet

```
https://sayman-faucet-site.vercel.app
```

---

# Requirements

* Node.js 18+
* npm 9+

---

# License

MIT License

Copyright © 2026 Vizkus Groups.

---

## Links

* Website: https://vizkusgroups.me
* Documentation: https://sayman-docs.vercel.app
* Explorer: https://sayman.onrender.com
* Faucet: https://sayman-faucet-site.vercel.app
* JavaScript SDK: https://www.npmjs.com/package/@sayman/sdk
* GitHub: https://github.com/saymanlal/SAYMAN

---

Built with ❤️ by **Vizkus Groups** for the **SAYMAN Blockchain** ecosystem.

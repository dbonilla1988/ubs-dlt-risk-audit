# 🔐 UBS DLT Risk Audit – Slither Static Analysis

This repository presents a static security audit conducted using [Slither](https://github.com/crytic/slither) on the [OpenZeppelin ERC20](https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC20/ERC20.sol) smart contract.

---

## 🛠️ Tools & Environment

- Slither v0.11.3
- Python 3.13.2
- Foundry (forge v1.4.3)
- solc-select (solc 0.8.27)
- macOS local setup

---

## 📄 Audit Scope

- Contract analyzed: `contracts/token/ERC20/ERC20.sol`
- Source: [OpenZeppelin Contracts](https://github.com/OpenZeppelin/openzeppelin-contracts)
- Solidity version: `^0.8.0`

---

## 🧪 Audit Command

```bash
slither contracts/token/ERC20/ERC20.sol --solc-remaps "@openzeppelin/=node_modules/@openzeppelin/" --disable-color > erc20-slither-report.md

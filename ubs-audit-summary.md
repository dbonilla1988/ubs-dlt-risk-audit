# 🔐 UBS DLT Risk Audit – Slither Static Analysis

This repository presents static security audit reports conducted using [Slither](https://github.com/crytic/slither) on key components of the [OpenZeppelin ERC20](https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC20/ERC20.sol) smart contract library. These reports are tailored for institutional audit readiness, including relevance to UBS tokenization and custody frameworks.

---

## 🛠️ Tools & Environment

| Tool          | Version        |
|---------------|----------------|
| Slither       | v0.11.3        |
| Python        | 3.13.2         |
| Foundry       | forge v1.4.3   |
| solc-select   | solc 0.8.27    |
| System        | macOS (local)  |

---

## 📄 Audit Scope

Contracts analyzed:

| Contract              | Description                    | Report Link                                 |
|-----------------------|--------------------------------|----------------------------------------------|
| `ERC20.sol`           | Core token logic               | [erc20-slither-report.md](./erc20-slither-report.md) |
| `ERC20Burnable.sol`   | Burn functionality (no minting)| [erc20-burnable-report.md](./erc20-burnable-report.md) |
| `ERC20Capped.sol`     | Max supply enforcement         | [erc20-capped-report.md](./erc20-capped-report.md)     |

---

## 🧪 Sample Audit Command

```bash
slither contracts/token/ERC20/extensions/ERC20Burnable.sol \
  --solc-remaps "@openzeppelin/=contracts/" \
  --disable-color \
  --print human-summary \
  > ~/ubs-dlt-risk-audit/erc20-burnable-report.md 2>&1

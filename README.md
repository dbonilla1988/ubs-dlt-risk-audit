# 🔐 UBS DLT Risk Audit – Slither Static Analysis

This repository contains a static security analysis using [Slither](https://github.com/crytic/slither) on the OpenZeppelin ERC20 contract.

### 📂 Tools & Environment

- Slither v0.11.3
- Python 3.13.2
- Foundry (forge v1.4.3)
- solc-select (auto-installed solc 0.8.27)
- macOS local setup

### 🚨 Key Finding

**Mixed Solidity Version Constraints Detected**

Slither flagged inconsistent pragma versions across multiple imported contracts (e.g., `>=0.8.4`, `^0.8.20`, `>=0.4.16`, etc.), which may impact audit reproducibility and deterministic builds in regulated CI/CD pipelines.

### 🧠 Institutional Relevance

This type of issue would be flagged within a smart contract risk control framework at institutions like UBS — especially for custody or tokenization systems requiring strict version enforcement.

---

📁 See `erc20-slither-report.md` for the full analysis output.

📌 Prepared by: **David Bonilla**

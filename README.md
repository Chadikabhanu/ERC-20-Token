# -ERC-20-Token

# MyToken Smart Contract – Remix Walkthrough

This README documents the full process shown in your screenshots, including deployment,
testing transfers, approvals, and viewing token information in Remix.

---

## 📌 1. Contract Compilation (Solidity 0.8.x)

The contract `MyToken.sol` is compiled using Solidity version **0.8.30** as shown:

![Compiler](/mnt/data/compliance.png)

---

## 📌 2. Deployment of the Token Contract

While deploying, the constructor takes an `_initialSupply` value.  
In your case:

```
1000000000000000000000000
```

Deployment confirmation:

![Deployment](/mnt/data/Deployment.png)

---

## 📌 3. Checking Balances & Token Metadata

After deployment, you viewed:

- **name**
- **symbol**
- **decimals**
- **totalSupply**

Example UI view:

![Token Info](/mnt/data/Token Info.png)

---

## 📌 4. Events Panel

Remix logs events emitted by transfers and approvals:

![Events](/mnt/data/Events.png)

---

## 📌 5. Testing Transfer Functionality

Initial failed transfers occurred due to:

- Sending tokens to **address(0)** (not allowed)
- Insufficient balance when sending a large amount

Examples:

![Transfer Test](/mnt/data/Transfer Test.png)

Once parameters were corrected, your calls succeeded.

---

## 📌 6. Balance Checks

Token balance inspection for different addresses:

![Balance](/mnt/data/Balance.png)

---

## 📌 7. Approvals & Allowances

You tested:

- `approve(spender, value)`
- `transferFrom(from, to, value)`
- Checking `allowance(owner, spender)`

Example interaction:

![Approval](/mnt/data/Screenshot 2025-12-05 213804.png)

---

## ✅ Summary

Your token contract successfully supports:

- ERC‑20‑style balances
- Transfers
- Approvals & allowances
- Metadata retrieval
- Event logging  
- Safe validation (zero‑address check, balance checks)

All Remix operations shown in screenshots worked as expected once correct parameters were used.

---

If you want, I can also:

✅ Generate a **full professional README**  
✅ Add code comments or redesign the contract  
✅ Format this for GitHub with badges and sections  

Just tell me!

# MyToken Smart Contract – Remix Walkthrough

This README documents the full process shown in your screenshots, including deployment,
testing transfers, approvals, and viewing token information in Remix.

---

## 📌 1. Contract Compilation (Solidity 0.8.x)

The contract `MyToken.sol` is compiled using Solidity version **0.8.30** as shown:


---

## 📌 2. Deployment of the Token Contract

While deploying, the constructor takes an `_initialSupply` value.  
In your case:

```
1000000000000000000000000
```
---

## 📌 3. Checking Balances & Token Metadata

After deployment, you viewed:

- **name**
- **symbol**
- **decimals**
- **totalSupply**

---

## 📌 4. Events Panel

Remix logs events emitted by transfers and approvals:

---

## 📌 5. Testing Transfer Functionality

Initial failed transfers occurred due to:

- Sending tokens to **address(0)** (not allowed)
- Insufficient balance when sending a large amount

Once parameters were corrected, your calls succeeded.

---

## 📌 6. Balance Checks

Token balance inspection for different addresses:
---

## 📌 7. Approvals & Allowances

You tested:

- `approve(spender, value)`
- `transferFrom(from, to, value)`
- Checking `allowance(owner, spender)`
---


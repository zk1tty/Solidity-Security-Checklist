# Solidity-Security-Checklist
Checklist for solidity contract deployment onto mainnet.

**When to conduct this checklist**

This checklist suppose to be conducted before code freezing.
However during integration test, and 

## Methodology

I start scanning solidity smart contracts to figure out top 1.0% common and critical vulnerabilities.

- How to list points:
    - Review the vulnerability report patterns from the top 10 projects within 2 months
- Concentrate on the top 1% of critical issues.
    - Check the pattern of vulnerability report from top 10 projects

### Vulnerability Severity Classification System
I refer to [the latest version(v2.3)](https://immunefi.com/immunefi-vulnerability-severity-classification-system-v2-3/) of Immunefi's vulnerability Severity Classification System.

4-levels of severity on each scope segment.

4-levels of Severity:
- Critical
- High
- Medium
- Low

Scope Segment:
- [Blockchain/DLT](./documents/Methodology.md#1-blockchaindlt)
- [Smart Contract](./documents/Methodology.md#2-smart-contracts)
- [WebApp](./documents/Methodology.md#3-websites-and-apps)

### Coverage
I filtered samples as the following criteria.
- Project Inherited ERC721 or ERC1155, and ERC2918(NFT Royalties).


### Policy

Keep it Simple, up to 10 points.

# CheckList
### 1. ReentrancyGuard

- function to input:

### 2. AccessControl

1. critical flow
2. extensional function for structs: tokenURI, 
3. Beneficiary of Royalty 

### 3.  Extensional operations

1. whitelist
2. royalty

### 4. External call after status udpate

- Pattern

### 5. Input Validation

### 6. Coverage of Operations

# References
Cited from the reports of following companies.

<img src="./assets/audit-company-logo/Immunefi-logo.png" width="250" height="60">
<img src="./assets/audit-company-logo/trail-of-bits-logo.png" width="250" height="60">
  
<img src="./assets/audit-company-logo/three-sigma-logo.png" width="250" height="60">
<img src="./assets/audit-company-logo/0xmacro-logo.png" width="250" height="60">

This checklist is inspired by [OWAPS-Web-Checklist](https://github.com/0xRadi/OWASP-Web-Checklist).
# Solidity-Security-Checklist
Checklist for solidity contract deployment onto mainnet

## Case: ERC721, ERC1155
### 1. **ReentrancyGuard**

- function to input:

### 2. **AccessControl**

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

This checklist is inspired by [OWAPS-Web-Checklist](https://github.com/0xRadi/OWASP-Web-Checklist).

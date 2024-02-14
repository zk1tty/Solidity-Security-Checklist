# Methodology
## Severity Classification System
### 1. Blockchain/DLT

4. Critical: Execute arbitrary system commands

- [ ] Retrieve sensitive data/files from a running server, such as:
    - [ ] /etc/shadow
    - [ ] database passwords
    - [ ] blockchain keys
(this does not include non-sensitive environment variables, open source code, or usernames)
- [ ] Taking down the application/website
- [ ] Taking down the NFT URI
- [ ] Taking state-modifying authenticated actions (with or without blockchain state interaction) on behalf of other users without any interaction by that user, such as:
    - [ ] Changing registration information
    - [ ] Commenting
    - [ ] Voting
    - [ ] Making trades
    - [ ] Withdrawals, etc.
- [ ] Changing the NFT metadata
- [ ] Subdomain takeover with already-connected wallet interaction
- [ ] Direct theft of user funds
- [ ] Malicious interactions with an already-connected wallet, such as:
    - [ ] Modifying transaction arguments or parameters
    - [ ] Substituting contract addresses
    - [ ] Submitting malicious transactions
- [ ] Direct theft of user NFTs
- [ ] Injection of malicious HTML or XSS through NFT metadata

### 2. Smart Contracts

### 3. Websites and Apps

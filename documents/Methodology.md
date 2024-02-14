# Methodology
## Severity Classification System
### 1. Blockchain/DLT

#### 1-1. Critical: Execute arbitrary system commands

#### 1-2. High: Execute arbitrary system commands

### 2. Smart Contracts
#### 2-1. Critical

- [ ] Manipulation of governance voting result deviating from voted outcome and resulting in a direct change from intended effect of original results
- [ ] Direct theft of any user funds, whether at-rest or in-motion, other than unclaimed yield
- [ ] Direct theft of any user NFTs, whether at-rest or in-motion, other than unclaimed royalties
- [ ] Permanent freezing of funds
- [ ] Permanent freezing of NFTs
- [ ] Unauthorized minting of NFTs
- [ ] Predictable or manipulable RNG that results in abuse of the principal or NFT
- [ ] Unintended alteration of what the NFT represents (e.g. token URI, payload, artistic content)
- [ ] Protocol insolvency

#### 2-2. High
- [ ] Theft of unclaimed yield
- [ ] Theft of unclaimed royalties
- [ ] Permanent freezing of unclaimed yield
- [ ] Permanent freezing of unclaimed royalties
- [ ] Temporary freezing of funds
- [ ] Temporary freezing NFTs

#### 2-3. Medium
- [ ] Smart contract unable to operate due to lack of token funds
- [ ] Block stuffing
- Griefing (e.g. no profit motive for an attacker, but damage to the users or the protocol)
- Theft of gas
- Unbounded gas consumption

#### 3-4. Low
- Contract fails to deliver promised returns, but doesn't lose value

### 3. Websites and Apps
#### 3-1. Critical

- [ ] Retrieve sensitive data/files from a running server, such as:
    - /etc/shadow
    - database passwords
    - blockchain keys
(this does not include non-sensitive environment variables, open source code, or usernames)
- [ ] Taking down the application/website
- [ ] Taking down the NFT URI
- [ ] Taking state-modifying authenticated actions (with or without blockchain state interaction) on behalf of other users without any interaction by that user, such as:
    - Changing registration information
    - Commenting
    - Voting
    - Making trades
    - Withdrawals, etc.
- [ ] Changing the NFT metadata
- [ ] Subdomain takeover with already-connected wallet interaction
- [ ] Direct theft of user funds
- [ ] Malicious interactions with an already-connected wallet, such as:
    - Modifying transaction arguments or parameters
    - Substituting contract addresses
    - Submitting malicious transactions
- [ ] Direct theft of user NFTs
- [ ] Injection of malicious HTML or XSS through NFT metadata

### 3-2. High

- [ ]  Injecting/modifying the static content on the target application without JavaScript (persistent), such as:
    -  HTML injection without JavaScript
    -  Replacing existing text with arbitrary text
    -  Arbitrary file uploads, etc.
- [ ]  Changing sensitive details of other users (including modifying browser local storage) without already-connected wallet interaction and with up to one click of user interaction, such as:
    -  Email or password of the victim, etc.
- [ ]  Improperly disclosing confidential user information, such as:
    -  Email address
    -  Phone number
    -  Physical address, etc.
- [ ]  Subdomain takeover without already-connected wallet interaction

### 3-3. Medium
- [ ] Changing non-sensitive details of other users (including modifying browser local storage) without already-connected wallet interaction and with up to one click of user interaction, such as:
    -  Changing the first/last name of user
    -  Enabling/disabling notifications
- [ ] Injecting/modifying the static content on the target application without JavaScript (reflected), such as:
    -  Reflected HTML injection
    -  Loading external site data
- [ ]  Redirecting users to malicious websites (open redirect)

### 3-4. Low

- [ ]  Changing details of other users (including modifying browser local storage) without already-connected wallet interaction and with significant user interaction, such as:
    -  Iframing leading to modifying the backend/browser state (must demonstrate impact with PoC)
- [ ]  Taking over broken or expired outgoing links, such as:
    -  Social media handles, etc.
- [ ]  Temporarily disabling user to access target site, such as:
    -  Locking up the victim from login
    - [ ]  Cookie bombing, etc.


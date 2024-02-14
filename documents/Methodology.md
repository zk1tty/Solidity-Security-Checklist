# Methodology
## Severity Classification System
### 1. Blockchain/DLT

#### 1-1. Critical
- [ ] Network not being able to confirm new transactions (total network shutdown)
- [ ] Unintended permanent chain split requiring hard fork (network partition requiring hard fork)
- [ ] Direct loss of funds
- [ ] Permanent freezing of funds (fix requires hardfork)

#### 1-2. High
- [ ] Unintended chain split (network partition)
- [ ] Temporary freezing of network transactions by delaying one block by 500% or more of the average block time of the preceding 24 hours beyond standard difficulty adjustments
- [ ] Causing network processing nodes to process transactions from the mempool beyond set parameters
- [ ] RPC API crash affecting projects with greater than or equal to 25% of the market capitalization on top of the respective layer

#### 1-3. Medium
- [ ] Increasing network processing node resource consumption by at least 30% without brute force actions, compared to the preceding 24 hours
- [ ] Shutdown of greater than or equal to 30% of network processing nodes without brute force actions, but does not shut down the network
- [ ] A bug in the respective layer 0/1/2 network code that results in unintended smart contract behavior with no concrete funds at direct risk

#### 1-4. Low
- [ ] Shutdown of greater than 10% or equal to but less than 30% of network processing nodes without brute force actions, but does not shut down the network
- [ ] Modification of transaction fees outside of design parameters

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
- [ ] Griefing (e.g. no profit motive for an attacker, but damage to the users or the protocol)
- [ ] Theft of gas
- [ ] Unbounded gas consumption

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

#### 3-2. High

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

#### 3-3. Medium
- [ ] Changing non-sensitive details of other users (including modifying browser local storage) without already-connected wallet interaction and with up to one click of user interaction, such as:
    -  Changing the first/last name of user
    -  Enabling/disabling notifications
- [ ] Injecting/modifying the static content on the target application without JavaScript (reflected), such as:
    -  Reflected HTML injection
    -  Loading external site data
- [ ]  Redirecting users to malicious websites (open redirect)

#### 3-4. Low

- [ ]  Changing details of other users (including modifying browser local storage) without already-connected wallet interaction and with significant user interaction, such as:
    -  Iframing leading to modifying the backend/browser state (must demonstrate impact with PoC)
- [ ]  Taking over broken or expired outgoing links, such as:
    -  Social media handles, etc.
- [ ]  Temporarily disabling user to access target site, such as:
    -  Locking up the victim from login
    - [ ]  Cookie bombing, etc.


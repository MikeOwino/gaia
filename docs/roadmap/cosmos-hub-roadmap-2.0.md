# The Cosmos Hub Roadmap 2.0

This Cosmos Hub Product Roadmap incorporates input from product owners, key Cosmos stakeholders (ATOM holders, Interchain Foundation, and Cosmos Hub operations), the internal Gaia / ATOM call, the virtual Gaia Org Call, the [Cosmos Hub as a Port City](https://blog.cosmos.network/the-cosmos-hub-is-a-port-city-5b7f2d28debf) article, and the [ATOM2021](https://github.com/cosmosdevs/atom2021) presentation.

This roadmap gives a one-year guideline in which stakeholders can anticipate updated features on the Cosmos Hub, with the greatest degree of specificity available for the most immediate upgrades, and decreasing precision available the further out the timeline goes. For example, the roadmap is most precise for the upcoming Liquidity upgrades (the Gravity DEX and Gravity Bridge modules).

The upgrades aim to add features such as liquidity, economic security, usability, and participation. To highlight our focus on DeFi, we have chosen to use the [Greeks from Finance](https://en.wikipedia.org/wiki/Greeks_(finance)) in naming upcoming upgrades.

## Delta Upgrade (Completed July 12, 2021)

- Gravity DEX:
  - A scalable AMM model for token swaps
  - Drives liquidity for tokens on the Cosmos Hub
  - Delivers price consistency and order execution

## Vega Upgrade (expected Q4 2021)

 - Cosmos SDK v0.44
   - Fee grant module:
      - Allows paying fees on behalf of another account
   - Authz module:
      - Provide governance functions to execute transactions on behalf of another account
- Liquidity Module v1.4.2
  -  The Gravity DEX with updates for dependencies
 - IBC v2.0.0
 - Tendermint v0.34.14
 - Cosmosvisor v0.1.0
 - IBC packet forward middleware v1.0.1

## Theta Upgrade (expected Q1 2022)

- Cosmos SDK v0.45
  - Groups module:
    - Enables higher-level multisig permissioned accounts, e.g., weight-based voting policies
  - Meta-Transactions
    - Allows transactions to be submitted by separate accounts that receive tips.
  - Gov Module Improvements
    - Execution of arbitraty transactions instead of just governance proposals.
    - Enables much more expressive governance module.
- NFT module
  - Enable simple management of NFT identifiers, their owners, and associated data, such as URIs, content, and provenance
  - An extensible base module for extensions including collectibles, custody, provenance, and marketplaces
- Tendermint v0.35
- Interchain accounts
  - A requirement in order to manage accounts across multiple blockchains
  - Aims to provide locking/unlocking mechanisms across IBC-enabled blockchains
  - Would allow custody providers to service any IBC connected blockchain through a common interface on the Hub.
- Liquid Staking
  - Frees secure and low-risk delegations for use in other parts of the Cosmos ecosystem
  - Features include enabling transfer of rewards and voting rights
- Items still being discussed:
  - Governance permissioned CosmWASM instance on the hub
  - Cosmos <> Ethereum Gravity Bridge
    - Transfer ATOM, ETH, ERC-20, and tokens on the Cosmos Hub between Ethereum- and Cosmos-compatible chains  
    - Fee and reward model hosted across Cosmos and Ethereum
    - Adds light-weight infrastructure and operational requirements with minimal slashing conditions to all Hub validators
  - Budget Module
    - Inflation funding directed to arbitrary module and account addresses
  - Farming Module
    - Rewards for locked tokens, especially LP tokens for different trading pair pools

## Rho Upgrade (expected Q2 2022)

- Interchain Security v1 - Required Participation of Provider Chain Validators
  - The Cosmos solution to shared security that uses IBC Cross Chain Validation (CCV) to relay validator set composition from a Provider Chain (Cosmos Hub) to a Consumer Chain. This validator set is in charge of producing blocks on both networks using separate nodes. Misbehavior on the Consumer Chain results in slashing Provider Chain staking tokens (ATOM).
  - Allows independent modules like Gravity DEX or Bridge to live on separate chains with their own development cycles.
- Chain Name Service
  -  Chain-ID registry
    - Node registry
    - IBC Path Resolution
  -  Asset registry
  -  Account registry
  -  Bech32 registry


## Lambda Upgrade (expected Q3 2022)

- Interchain Security v2 - Opt-In Participation of Provider Chain Validators
  - Where Provider Chain validators have the ability to opt-in to block production for various Consumer Chains.
- Cosmos SDK v0.46
  - SMT
  - Postgres indexing
  - Protobuf v2
- Token Issuance
  - Enables creation of tokens directly on the Hub
  - Aims to provide ERC20 capabilities
- Gravity DEX v2
  - Order matching

## Epsilon (expected Q4 2022)

- Interchain Security v3 - Layered Security
  - Where Consumer Chains combine their own staking token validator set with Provider Chain validator set.

## Future Upgrades

- Cross-chain bridges (non-IBC)
- Atomic Exchange
- Decentralized identifiers (DID)
- Privacy
- Virtual machines
- Smart contract languages
- Zero knowledge and optimistic rollups

The Cosmos Hub Roadmap is maintained by the Interchain Cosmos Hub team as a living document, and is updated in collaboration with key stakeholders from the multi-entity Cosmos community. 

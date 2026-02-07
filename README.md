# Udacity Blockchain Developer Nanodegree Projects

This repository collects my work across the Udacity Blockchain Developer Nanodegree. Each project lives in its own folder and includes its own README with setup and submission notes where applicable.

## Projects

* [Project 1 - Blockchain Identity](Project%201%20-%20Blockchain%20Identity)
* [Project 2 - Blockchain Data](Project%202%20-%20Blockchain%20Data)
* [Project 3 - Blockchain Web Services](Project%203%20-%20Blockchain%20Web%20Services)
* [Project 4 - Private Blockchain Notary Service](Project%204%20-%20Private%20Blockchain%20Notary%20Service)
* [Project 5 - Identity and Smart Contracts](Project%205%20-%20Identity%20and%20Smart%20Contracts)
* [Project 6 - Blockchain Architecture Part A](Project%206%20-%20Blockchain%20Architecture%20Part%20A)
* [Project 7 - Blockchain Architecture Part B](Project%207%20-%20Blockchain%20Architecture%20Part%20B)
* [Project 8 - Advanced Blockchain Concepts and Oracles](Project%208%20-%20Advanced%20Blockchain%20Concepts%20and%20Oracles)
* [Project 9 - Capstone (Real Estate Marketplace)](Project%209%20-%20Capstone%20Project)

## Topics covered

- Blockchain fundamentals (hashing, blocks, validation, persistence)
- REST APIs for blockchain services
- Smart contracts and tokenization
- Supply chain dApps and access control
- Oracle patterns and advanced contract architecture
- Capstone delivery and on-chain verification

## Project details

### Project 1 - Blockchain Identity
Builds a simple blockchain and lets users register and validate identities. Focuses on block structure, hashing, ownership proofs, and basic validation workflows.

### Project 2 - Blockchain Data
Implements a persistent blockchain with LevelDB. Adds block validation, chain validation, and database-backed storage for blocks and metadata.

### Project 3 - Blockchain Web Services
Exposes blockchain functionality via a REST API. Includes endpoints for block lookup and creation, and demonstrates API design and data validation.

### Project 4 - Private Blockchain Notary Service
Extends the web service with a mempool, wallet-based identity, and star registry/notary flow. Introduces time-bound validation windows and signed message verification.

### Project 5 - Identity and Smart Contracts
Implements an ERC-721 star registry. Covers smart contract deployment, token minting, ownership transfer, and basic on-chain metadata.

### Project 6 - Blockchain Architecture Part A
Architecture and design documentation: diagrams and system modeling artifacts for a supply chain solution.

### Project 7 - Blockchain Architecture Part B
Builds a supply chain dApp with role-based access control and event-driven workflows. Includes Solidity contracts, migrations, and tests.

### Project 8 - Advanced Blockchain Concepts and Oracles
Implements the FlightSurety contracts and oracle flow. Covers multi-party consensus, data oracles, and dApp integration.

### Project 9 - Capstone (Real Estate Marketplace)
Capstone combining zk-SNARK verification with ERC-721 minting. Demonstrates proof verification, mint authorization, and marketplace-ready metadata.

## Tooling and stack (varies per project)

- Node.js and npm
- LevelDB
- Express
- Web3, Truffle, Ganache
- Solidity

## Getting started

1) Pick a project folder from the list above.
2) Read the project README for prerequisites and setup steps.
3) Install dependencies within that project folder:
   ```
   npm install
   ```
4) Run the project based on its README instructions (some projects are CLI-only, others are web services or dApps).

## Notes

- Project folders are self-contained and may use different dependencies or node versions.
- Some projects include compiled artifacts or diagrams that are part of submissions.

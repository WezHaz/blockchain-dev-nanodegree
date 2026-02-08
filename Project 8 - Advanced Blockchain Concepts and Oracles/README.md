# Project #8. Advanced Blockchain Concepts and Oracles

## Overview

FlightSurety is a sample dApp that demonstrates oracle-driven workflows and multi-party consensus patterns in Solidity. It includes smart contracts, a server for oracle simulation, and a front-end dApp.

## Objectives

- Implement a multi-contract architecture (data + app contracts)
- Require multi-party consensus for airline registration
- Use oracles to supply external data to the contract
- Build a simple dApp to buy insurance and view flight status

## Install

This repository contains Smart Contract code in Solidity (using Truffle), tests (also using Truffle), dApp scaffolding (using HTML, CSS and JS) and server app scaffolding.

To install, download or clone the repo, then:

`npm install`
`truffle compile`

## Develop Client

To run truffle tests:

`truffle test ./test/flightSurety.js`
`truffle test ./test/oracles.js`

To use the dapp:

`truffle migrate`
`npm run dapp`

To view dapp:

`http://localhost:8000`

## Develop Server

`npm run server`
`truffle test ./test/oracles.js`

## Deploy

To build dapp for prod:
`npm run dapp:prod`

Deploy the contents of the ./dapp folder


## Key files

- `contracts/FlightSuretyData.sol` — data contract with persistence
- `contracts/FlightSuretyApp.sol` — app contract with business logic
- `src/server/server.js` — oracle simulation server
- `src/dapp/` — front‑end client
- `test/flightSurety.js` — contract tests
- `test/oracles.js` — oracle flow tests

## Notes

- Run both the server and dApp for the full flow.
- Oracle tests require Ganache (or Truffle Develop) with funded accounts.
- The solidity version in this project is pinned; if you upgrade, update Truffle config and contracts.

## Resources

* [How does Ethereum work anyway?](https://medium.com/@preethikasireddy/how-does-ethereum-work-anyway-22d1df506369)
* [BIP39 Mnemonic Generator](https://iancoleman.io/bip39/)
* [Truffle Framework](http://truffleframework.com/)
* [Ganache Local Blockchain](http://truffleframework.com/ganache/)
* [Remix Solidity IDE](https://remix.ethereum.org/)
* [Solidity Language Reference](http://solidity.readthedocs.io/en/v0.4.24/)
* [Ethereum Blockchain Explorer](https://etherscan.io/)
* [Web3Js Reference](https://github.com/ethereum/wiki/wiki/JavaScript-API)

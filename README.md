# Truffle version

* truffle version
* Truffle v5.4.29 (core: 5.4.29)
* Solidity - ^0.4.24 (solc-js)
* Node v16.17.1
* Web3.js v1.5.3

# FlightSurety

FlightSurety is a sample application project for Udacity's Blockchain course.

## Install

This repository contains Smart Contract code in Solidity (using Truffle), tests (also using Truffle), dApp scaffolding (using HTML, CSS and JS) and server app scaffolding.

To install, download or clone the repo, then:

`npm install`
`truffle compile`
```bash
truffle compile

Compiling your contracts...
===========================
√ Fetching solc version list from solc-bin. Attempt #1
√ Fetching solc version list from solc-bin. Attempt #1
> Compiling .\contracts\FlightSuretyApp.sol
> Compiling .\contracts\FlightSuretyApp.sol
> Compiling .\contracts\FlightSuretyData.sol
> Compiling .\contracts\FlightSuretyData.sol
> Compiling .\contracts\Migrations.sol
> Artifacts written to E:\Blockchain_Developer\newnewProject4\FlightSurety-master\build\contracts
> Compiled successfully using:
   - solc: 0.4.26+commit.4563c3fc.Emscripten.clang
```
## Develop Client

To run truffle tests:

`truffle test ./test/flightSurety.js`
`truffle test ./test/oracles.js`

To use the dapp:

`truffle migrate`
```bash
PS E:\Blockchain_Developer\newnewProject4\FlightSurety-master> truffle migrate

Compiling your contracts...
===========================
√ Fetching solc version list from solc-bin. Attempt #1
√ Fetching solc version list from solc-bin. Attempt #1
> Compiling .\contracts\FlightSuretyApp.sol
> Compiling .\contracts\FlightSuretyData.sol
> Compiling .\contracts\FlightSuretyData.sol
> Compiling .\contracts\Migrations.sol
> Artifacts written to E:\Blockchain_Developer\newnewProject4\FlightSurety-master\build\contracts
> Compiled successfully using:
   - solc: 0.4.26+commit.4563c3fc.Emscripten.clang

 
Starting migrations...
======================
> Network name:    'development'
> Network id:      5777
> Block gas limit: 300000000 (0x11e1a300)


1_initial_migration.js
======================

   Deploying 'Migrations'
   ----------------------
   > transaction hash:    0xc0ae9998cc38d3e037db67d3b7d316d5ae92a7d3d221d275c80f0f68b5087a38
   > Blocks: 0            Seconds: 0
   > contract address:    0xbd23b6ce173D388128f9C9f623a11D36b10700A6
   > block number:        16
   > block timestamp:     1671650444
   > account:             0xFF138eF85a7e96ac9702E3fdD08C98934bEC9e5a
   > balance:             99.62810516
   > gas used:            238594 (0x3a402)
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.00477188 ETH


   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:          0.00477188 ETH


2_deploy_contracts.js
=====================

   Deploying 'FlightSuretyData'
   ----------------------------
   > transaction hash:    0x757e6653e1a49b86813db38142bf7ab8dc40e265337a098f9410dc945783c89a
   > Blocks: 0            Seconds: 0
   > contract address:    0x667343E1a7F52fC269866b9DeA63d22F781c6710
   > block number:        18
   > block timestamp:     1671650447
   > account:             0xFF138eF85a7e96ac9702E3fdD08C98934bEC9e5a
   > balance:             99.5688727
   > gas used:            2919275 (0x2c8b6b)
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.0583855 ETH


   Deploying 'FlightSuretyApp'
   ---------------------------
   > transaction hash:    0x04c17ebfe4cb4d0d23742c83fe43028f61983beb8fe051e7fc4814dbd206bbbb
   > Blocks: 0            Seconds: 0
   > contract address:    0x19771509c13C57A0bCb176e7f103D1212A3a2122
   > block number:        19
   > block timestamp:     1671650448
   > account:             0xFF138eF85a7e96ac9702E3fdD08C98934bEC9e5a
   > balance:             99.51104528
   > gas used:            2891371 (0x2c1e6b)
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.05782742 ETH


   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:          0.11621292 ETH


Summary
=======
> Total deployments:   3
> Final cost:          0.1209848 ETH

```

`npm run dapp`
npm run dapp
![npm run dapp](images/npmRunDapp.png)
> flightsurety@1.0.0 dapp
> webpack-dev-server --mode development --config webpack.config.dapp.js

i ｢wds｣: Project is running at http://localhost:8000/
i ｢wds｣: webpack output is served from /
i ｢wds｣: Content not from webpack is served from E:\Blockchain_Developer\newnewProject4\FlightSurety-master\dapp
i ｢wdm｣:    881 modules
i ｢wdm｣: Compiled successfully.
i ｢wdm｣: Compiling...
i ｢wdm｣:    881 modules


To view dapp:

`http://localhost:8000`

## Develop Server

`npm run server`
`truffle test ./test/oracles.js`

## Deploy

To build dapp for prod:
`npm run dapp:prod`

Deploy the contents of the ./dapp folder


## Resources

* [How does Ethereum work anyway?](https://medium.com/@preethikasireddy/how-does-ethereum-work-anyway-22d1df506369)
* [BIP39 Mnemonic Generator](https://iancoleman.io/bip39/)
* [Truffle Framework](http://truffleframework.com/)
* [Ganache Local Blockchain](http://truffleframework.com/ganache/)
* [Remix Solidity IDE](https://remix.ethereum.org/)
* [Solidity Language Reference](http://solidity.readthedocs.io/en/v0.4.24/)
* [Ethereum Blockchain Explorer](https://etherscan.io/)
* [Web3Js Reference](https://github.com/ethereum/wiki/wiki/JavaScript-API)

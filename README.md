# ND1309 C2 Ethereum Smart Contracts, Tokens and Dapps - Project Starter 
**PROJECT: Decentralized Star Notary Service Project** - For this project, you will create a DApp by adding functionality with your smart contract and deploy it on the public testnet.

### Summary and Token Infomation
This Starter Code has already implemented the functionalities you implemented in the StarNotary (Version 2) exercise, and have comments in all the files you need to implement your tasks.The project is built upon the boiler plate code provided for a Star Notary service utilising the ERC-721 standard. It is deployed on the Rinkeby Ethereum Testnet with the following details:

* Token Name: Star Token 
* Token Symbol: STC
* Contract Address: 0x59cDc607cb8B9100a080ED9f474799ED00432924
* EtherScan Location: https://rinkeby.etherscan.io/token/0x59cdc607cb8b9100a080ed9f474799ed00432924?a=0xE8E2352988c97a32FB0405486A29b48cF7942e42
* Transactions: https://rinkeby.etherscan.io/address/0xE8E2352988c97a32FB0405486A29b48cF7942e42
* Node version: v16.13.0
* Truffle version:Truffle v5.5.21 - a development framework for Ethereum
* OpenZeppelin version: 2.3.0

#### Rinkby Delpoyment output
(base) PS F:\Udacity BlockChain\Udacity BlockChain Projects\nd1309-p2-Decentralized-Star-Notary-Service-Starter-Code-main\nd1309-p2-Decentralized-Star-Notary-Service-Starter-Code-main> truffle migrate --reset --network rinkeby

Compiling your contracts...
===========================
> Compiling .\app\node_modules\openzeppelin-solidity\contracts\drafts\Counters.sol
> Compiling .\app\node_modules\openzeppelin-solidity\contracts\introspection\ERC165.sol
> Compiling .\app\node_modules\openzeppelin-solidity\contracts\introspection\IERC165.sol
> Compiling .\app\node_modules\openzeppelin-solidity\contracts\math\SafeMath.sol
> Compiling .\app\node_modules\openzeppelin-solidity\contracts\token\ERC721\ERC721.sol
> Compiling .\app\node_modules\openzeppelin-solidity\contracts\token\ERC721\IERC721.sol
> Compiling .\app\node_modules\openzeppelin-solidity\contracts\token\ERC721\IERC721Receiver.sol
> Compiling .\app\node_modules\openzeppelin-solidity\contracts\utils\Address.sol
> Compiling .\contracts\Migrations.sol
> Compiling .\contracts\StarNotary.sol
> Artifacts written to F:\Udacity BlockChain\Udacity BlockChain Projects\nd1309-p2-Decentralized-Star-Notary-Service-Starter-Code-main\nd1309-p2-Decentralized-Star-Notary-Service-Starter-Code-main\build\contracts
> Compiled successfully using:
   - solc: 0.5.16+commit.9c3226ce.Emscripten.clang


Migrations dry-run (simulation)
===============================
> Network name:    'rinkeby-fork'
> Network id:      4
> Block gas limit: 29999972 (0x1c9c364)


1_initial_migration.js
======================

   Deploying 'Migrations'
   ----------------------
   > block number:        10994011
   > block timestamp:     1657368003
   > account:             0xE8E2352988c97a32FB0405486A29b48cF7942e42
   > balance:             0.09546926
   > gas used:            226537 (0x374e9)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.00226537 ETH

   -------------------------------------
   > Total cost:          0.00226537 ETH


2_deploy_contracts.js
=====================

   Deploying 'StarNotary'
   ----------------------
   > block number:        10994013
   > block timestamp:     1657368008
   > account:             0xE8E2352988c97a32FB0405486A29b48cF7942e42
   > balance:             0.07352329
   > gas used:            2148834 (0x20c9e2)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.02148834 ETH

   -------------------------------------
   > Total cost:          0.02148834 ETH

Summary
=======
> Total deployments:   2
> Final cost:          0.02375371 ETH




Starting migrations...
======================
> Network name:    'rinkeby'
> Network id:      4
> Block gas limit: 30000000 (0x1c9c380)


1_initial_migration.js
======================

   Deploying 'Migrations'
   ----------------------
   > transaction hash:    0xf7e6e249f92846cfc2237562894bfd040a7ae6961aff3a518b6142d34d407a2b
   > Blocks: 2            Seconds: 17
   > contract address:    0x6DbA7f9314a74c93413afCcC30b368fAa60E9b4B
   > block number:        10994018
   > block timestamp:     1657368039
   > account:             0xE8E2352988c97a32FB0405486A29b48cF7942e42
   > balance:             0.09546926
   > gas used:            226537 (0x374e9)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.00226537 ETH

   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:          0.00226537 ETH


2_deploy_contracts.js
=====================

   Deploying 'StarNotary'
   ----------------------
   > transaction hash:    0x38876da640679488fe1ee023fe821a0f6ba4abb772cbab206d020f6b5e423a02
   > Blocks: 1            Seconds: 9
   > contract address:    0x59cDc607cb8B9100a080ED9f474799ED00432924
   > block number:        10994020
   > block timestamp:     1657368069
   > account:             0xE8E2352988c97a32FB0405486A29b48cF7942e42
   > balance:             0.07352329
   > gas used:            2148834 (0x20c9e2)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.02148834 ETH

   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:          0.02148834 ETH

Summary
=======
> Total deployments:   2
> Final cost:          0.02375371 ETH


### Dependencies
For this project, you will need to have:
1. **Node and NPM** installed - NPM is distributed with [Node.js](https://www.npmjs.com/get-npm)
```bash
# Check Node version
node -v
# Check NPM version
npm -v
```


2. **Truffle v5.X.X** - A development framework for Ethereum. 
```bash
# Unsinstall any previous version
npm uninstall -g truffle
# Install
npm install -g truffle
# Specify a particular version
npm install -g truffle@5.0.2
# Verify the version
truffle version
```


2. **Metamask: 5.3.1** - If you need to update Metamask just delete your Metamask extension and install it again.


3. [Ganache](https://www.trufflesuite.com/ganache) - Make sure that your Ganache and Truffle configuration file have the same port.


4. **Other mandatory packages**:
```bash
cd app
# install packages
npm install --save  openzeppelin-solidity@2.3
npm install --save  truffle-hdwallet-provider@1.0.17
npm install webpack-dev-server -g
npm install web3
```


### Run the application
1. Clean the frontend 
```bash
cd app
# Remove the node_modules  
# remove packages
rm -rf node_modules
# clean cache
npm cache clean
rm package-lock.json
# initialize npm (you can accept defaults)
npm init
# install all modules listed as dependencies in package.json
npm install
```


2. Start Truffle by running
```bash
# For starting the development console
truffle develop
# truffle console

# For compiling the contract, inside the development console, run:
compile

# For migrating the contract to the locally running Ethereum network, inside the development console
migrate --reset

# For running unit tests the contract, inside the development console, run:
test
```

3. Frontend - Once you are ready to start your frontend, run the following from the app folder:
```bash
cd app
npm run dev
```

---

### Important
When you will add a new Rinkeyby Test Network in your Metamask client, you will have to provide:

| Network Name | New RPC URL | Chain ID |
|---|---|---|
|Private Network 1|`http://127.0.0.1:9545/`|1337 |

The chain ID above can be fetched by:
```bash
cd app
node index.js
```

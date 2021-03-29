# Ethereum Dapp for Tracking Items through Supply Chain

## Project Write-Up

### UML Diagrams
[Activity](./uml/activity.png)<br>
[Sequence](./uml/sequence.png)<br>
[State](./uml/state.png)<br>
[Classes (Data Model)](./uml/class.png)<br>
<br>

### Libraries
Library      | Version
------------ | -------------
Node             |v14.15.3
Solidity         |v0.5.16
Truffle          |v5.1.63
truffle-hdwallet-provider |v1.0.17
truffle-assertions   |v0.9.2
web3             |v1.2.1
lite-server      |v2.6.1


### Usage of Libraries
- **Solidity** is used for writing the smart contracts.

- **web3.js** allows to interact with the local Ganache and remote Rinkeby Ethereum node using HTTP, IPC or WebSocket.<br>

- **Truffle** is used to develop, migrate Solidity smart contracts to local Ganache Blockchain and to Rinkeby Ethereum network, and to test these smart contracts.

- **truffle-hdwallet-provider** is used to sign transactions for addresses derived from a 12-word mnemonic.

- **truffle-assertions** adds additional assertions for testing smart contracts inside Truffle tests.

- **lite-server** is a lightweight development only node server that is used to serve the frontend web app.




### IPFS
IPFS is not used in this project.<br>


### Compiling and Testing
Truffle and Ganache (personal blockchain) are used across the entire development cycle to develop, deploy, and test supply chain dApp in a safe and deterministic environment.

Staring Ganache by using Ganache command-line tool. Ganache will run at port 8545 (see networks:development in truffle.js):

ganache-cli -m  <12-word mnemonic>

`truffle develop`

`truffle> compile`

`truffle> migrate --reset`

`truffle> test`

<br>


### Deploying Smart Contracts on Rinkeby Public Test Network

`truffle migrate --network rinkeby --reset`

<br>


### Transaction IDs and Contract Addresses
Contract          | Transaction ID                                                      |  Contract Address
----------------- | --------------------------------------------------------------------|---------------------------------------------
FarmerRole        | [0xb6a3932652fc4204ce7638256c6fd2c3d1cf5938e340e830ead84f7c1855936b](https://rinkeby.etherscan.io/tx/0xb6a3932652fc4204ce7638256c6fd2c3d1cf5938e340e830ead84f7c1855936b)  | [0xc792f2b5b6f714d8d8656826215aa66afd01d007](https://rinkeby.etherscan.io/address/0xc792f2b5b6f714d8d8656826215aa66afd01d007#code)
DistributorRole   | [0x28069f37aa56db2720b26c6fdfc5bd2af73205bad555ba3eac9f8bfa26626896](https://rinkeby.etherscan.io/tx/0x28069f37aa56db2720b26c6fdfc5bd2af73205bad555ba3eac9f8bfa26626896)  | [0x51f42A1ED90CA6b3eea169c6c3dC61bd21E46840](https://rinkeby.etherscan.io/address/0x51f42A1ED90CA6b3eea169c6c3dC61bd21E46840#code)
RetailerRole      | [0x7b715d06db7b3cea4f649cb430469ad1324762323160e15a7f063cffa551dc7a](https://rinkeby.etherscan.io/tx/0x7b715d06db7b3cea4f649cb430469ad1324762323160e15a7f063cffa551dc7a)  | [0xd2cBE3A2E7a617A4252Bd24AfBEee0503F86Ec0b](https://rinkeby.etherscan.io/address/0xd2cBE3A2E7a617A4252Bd24AfBEee0503F86Ec0b#code)
ConsumerRole      | [0xd8677acd10be6dd775de0d3c2f750ec76f5a2334662aef21c520e9870752d59c](https://rinkeby.etherscan.io/tx/0xd8677acd10be6dd775de0d3c2f750ec76f5a2334662aef21c520e9870752d59c)  | [0x83690F2c1f9067d285a8954FE77b84f2054D61ef](https://rinkeby.etherscan.io/address/0x83690F2c1f9067d285a8954FE77b84f2054D61ef#code)
SupplyChain       | [0xe9d092e2141e10fa1b948b0dca44bd4c1ac564d15cddae3f64f8e0bb250ca121](https://rinkeby.etherscan.io/tx/0xe9d092e2141e10fa1b948b0dca44bd4c1ac564d15cddae3f64f8e0bb250ca121)  | [0x620Ae3f809843B70E1e31C857111D1EC7288755f](https://rinkeby.etherscan.io/address/0x620Ae3f809843B70E1e31C857111D1EC7288755f#code)

<br>

### Front-end
Front-end code was modified to use Bootstrap styling.


### Launching Web Server

Open a separate terminal window to launch the DApp:

`npm run dev`











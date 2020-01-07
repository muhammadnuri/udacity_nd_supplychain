## Project Write-Up - UML

- [Data Model Diagram](./uml/nd1309_supply_chain_data_model.png)
- [Activity Diagram](./uml/nd1309-supply-chain-activity.png)
- [Sequence Diagram](./uml/nd1309-supply-chain-sequence.png)
- [State Diagram](./uml/nd1309-supply-chain-state.png)

## Project Write-Up - Libraries

- Truffle v4.1.16 (core: 4.1.16): Development, testing and migration of smart contract.
- Solidity v0.4.26 (solc-js): Solidity compiler.
- Node v10.17.0: Node JS runtime.

## Rinkeby Migration

```
truffle migrate --reset --network rinkeby
Using network 'rinkeby'.

Running migration: 1_initial_migration.js
  Replacing Migrations...
  ... 0xa54b1a091f518104177d5a663de62ad2b33174523e3c497d43d25d4e4a5f9887
  Migrations: 0x0768e3b6daf9940e385d4e7b220304dc878ff11e
Saving successful migration to network...
  ... 0x2d1f1fad9ad5dcc106d73b8188037e0a2285712779a9730d8e741d3337f3abe3
Saving artifacts...
Running migration: 2_deploy_contracts.js
  Replacing FarmerRole...
  ... 0x07b57e4d2d0607b7a315239328a3ab2fd662b0570cd8145dd85a5c11cec7ce91
  FarmerRole: 0xe94b575ee71e2629af824dc70ca8c86819a03741
  Replacing DistributorRole...
  ... 0x71617f37b38db9fdc91041ba5872a0466a741708766c0b608cfdce0372de6740
  DistributorRole: 0xb8e3425ca7c9628b688a4d8a73f88945af5b1c90
  Replacing RetailerRole...
  ... 0x3216b41187cb9cd9721412607b7f0058896e2fd76fd5e8aa14cb57012fa554ff
  RetailerRole: 0x7cfc0f7fb8b7cc10a4481b37a881431f5a15060a
  Replacing ConsumerRole...
  ... 0xfb0b7c910c86c4da9c1bda50a539c3f30760f9838cf6c1f2c99c4631085b0ee1
  ConsumerRole: 0x3920d2d3f5c60b06c0acd5f43305c57a7b009e6a
  Replacing SupplyChain...
  ... 0xd53e9d0d67368acc282e1bbdcf4bb0aee36306a2d79d73c5c213a32a3e1eda0f
  SupplyChain: 0x1946156e22cf5349d4a9dda6410d7873f1e64917
Saving successful migration to network...
  ... 0xa21ca77c0130f446a5f753f4bb7cd025761974cc1c6ff3fee2de791e18230620
Saving artifacts...
```

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

Please make sure you've already installed ganache-cli, Truffle and enabled MetaMask extension in your browser.

```
Give examples (to be clarified)
```

### Installing

A step by step series of examples that tell you have to get a development env running

Clone this repository:

```
git clone https://github.com/muhammadnuri/udacity_nd_supplychain.git
```

Change directory to ```udacity_nd_supplychain``` folder and install all requisite npm packages (as listed in ```package.json```):

```
npm install
```

Launch Ganache:

```
ganache-cli -m "spirit supply whale amount human item harsh scare congress discover talent hamster"
```

Your terminal should look something like this:

![truffle test](images/ganache-cli.png)

In a separate terminal window, Compile smart contracts:

```
truffle compile
```

Your terminal should look something like this:

![truffle test](images/truffle_compile.png)

This will create the smart contract artifacts in folder ```build\contracts```.

Migrate smart contracts to the locally running blockchain, ganache-cli:

```
truffle migrate
```

Your terminal should look something like this:

![truffle test](images/truffle_migrate.png)

Test smart contracts:

```
truffle test
```

All 10 tests should pass.

![truffle test](images/truffle_test.png)

In a separate terminal window, launch the DApp:

```
npm run dev
```

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
truffle migrate --network rinkeby
Using network 'rinkeby'.

Running migration: 1_initial_migration.js
  Deploying Migrations...
  ... 0xc321dd003fb4e1451e6f67dc28162a6f94cf989975c70e7f79e775bb86b2532a
  Migrations: 0x30a9510d210f16453b15b308a095e42423e8d7dd
Saving successful migration to network...
  ... 0x5d51dea3d75b103812fe32519211560da22e42e2bc3135d0a21d4ee5dfc5fe08
Saving artifacts...
Running migration: 2_deploy_contracts.js
  Deploying FarmerRole...
  ... 0xba8beef8b99d067d63b8a2009299c54995a114f1740648370e9c65763da92e76
  FarmerRole: 0xc798983907c3f8dfda73a297aadc171f99e28011
  Deploying DistributorRole...
  ... 0x9a7e6b43e8f9da96b57abe0acb040a48e558b51278b4eeffb83544b144e82a6d
  DistributorRole: 0xd5a7fd7f332216550d87e938af5a9b506d51440c
  Deploying RetailerRole...
  ... 0xe07a8029d1c70f5de2fa273b78a4221695c83866640ea27c4b07e179f26ffa02
  RetailerRole: 0x5f2c9e3aa524fd9a1ee07f798ff87ce3db5c1bd4
  Deploying ConsumerRole...
  ... 0x23ff286d2dee7fd8e50ca372dc65b188cc1bd138fb8a38023966610292f45bc2
  ConsumerRole: 0x9e2c9f4f1a0a29e602d521f7f7ef6ac399b7719f
  Deploying SupplyChain...
  ... 0x5fb4f7f9836fe3ac45c606d99cd4340d204122b6a42c292c7e650b333f1d9e21
  SupplyChain: 0xf8da40da57ddbaafdef9ebb9555f77d6c214ab61
Saving successful migration to network...
  ... 0x70c4cac85b7c02115e9ba5bed4b528c1f2a7851801d69b9dcb6cdd21cd5a1a18
Saving artifacts...
```

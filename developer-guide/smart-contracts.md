# Smart Contracts

## Solidity

Currently the Trust is using a standard EVM implementation. Therefore all existing solidity compilers targeting standard EVM environment should work.&#x20;

There might be some limitations in the smart contracts. Please check [evm-compatibility.md](../understanding-trust/compatibility/evm-compatibility.md "mention") for more information.&#x20;

In the future, we might develop add-ons to the VM of the Trust EVM to support more features. In that case, one may need to use our SDK for development. We will update this guild if that happens.

## TruffleSuite

[Truffle](https://www.trufflesuite.com/) is a widely used development environment and testing framework for Ethereum smart contracts. Thanks to the architecture of the Trust EVM, all the existing SDKs for Ethereum will work out of the box and your users will have the same experience as on Ethereum.

Therefore, the official tutorials of Truffle applies to our Trust EVM perfectly:&#x20;

[https://trufflesuite.com/docs/truffle/quickstart/](https://trufflesuite.com/docs/truffle/quickstart/)\
\
The only difference would be don't forget to modify the config in `truffle-config.js`  file:

```
module.exports = {
  networks: {
  // Use the address of your favorite endpoint.
    trustevm: {
      host: "api.testnet-dev.trust.one",
      port: 15555,
      network_id: "*"
    }
  }
};

```

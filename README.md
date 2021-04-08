# Zinc Playground

In order to learn what I can do on zkSync and how I can develop smart contracts on zkSync, I put my progress in this repository. For now, I try to develop contracts of ERC20, ERC721, and NFTMarket on zkSync Rinkeby testnet.

[zkSync](https://zksync.io/) is a Layer-2 solution for Ethereum using zk rollup. This platform is going to allow developers to write smart contracts with Zinc Language. It is a vering promising project. Many DeFi protocols have join this ecosystem.

[Zinc](https://zinc.zksync.io/index.html) is an emerging framework for developing smart contracts and SNARK circuits on the zkSync platform.

## How to use

1. Install Zinc from [here](https://github.com/matter-labs/zinc)
2. Go to folders in which you are interested, e.g. `/erc20`.
3. Change an unique contract name in `Zargo.toml` file.
4. Compile smart contracts by running `zargo build`.
5. Setting parameters in `**/data/input.json`.
6. Deploy smart constracts by running `zargo publish --network rinkeby --instance default`.
7. Query the contract storage by running `zargo query --network rinkeby --address <contract-address>` or `zargo query --network rinkeby --address <contract-address> --method <method-name>`.
8. Call the contract method by running `zargo call --network rinkeby --address <contract-address> --method <method-name>`.

## Workaround solutions for some issues

This issues may be fixed or removed when offical team releases turing-compelte version of Zinc language.

- store string
- allowances mapping
- store IPFS hash using Uint8Array
- Intrinsic function: transfer
- asset porting between L1 and L2

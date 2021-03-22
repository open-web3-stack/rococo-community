# Community Rococo

This is an open community Rococo parachain testnet. The goal is to expedite parachain testing, and lower the overhead with shared infrastructure.

# The Network
- Connect to Community-Rococo via [Polkadot-JS Web App](https://polkadot.js.org/apps/?rpc=wss%3A%2F%2Frococo-community.laminar.codes#/explorer).
- RPC endpoint: [wss://rococo-community-rpc.laminar.codes/ws](https://polkadot.js.org/apps/?rpc=wss://rococo-community-rpc.laminar.codes/ws#/explorer)
- Bootnode: `/ip4/3.1.243.130/tcp/30335/p2p/12D3KooWLdZ4NrFaHPeUJqzafC5mD6StGezcWMoR9f4oRGyyiBDS`
- Chain spec: [rococo-community.json](./rococo-community.json)

## Run with Docker

```bash
docker run \
  -p 9944:9944 \
  -v $(pwd)/rococo-community.json:/rococo-community.json \
  parity/rococo:rococo-v1-0.8.29-2f7b9750-ad9db415 --chain=/rococo-community.json \
  --ws-external \
  --rpc-cors=all \
  --rpc-methods=Unsafe \
  --wasm-execution=Compiled
```

# Join as a Parachain
## Faucet

Please post your details to https://github.com/open-web3-stack/rococo-community/discussions/2

## Collator dependencies

Those commits are used by Acala collator. Other commit may or may not work.

- Polkadot: `2f7b975015d5c3f50199cda82b9b84e38726d001`
- Cumulus: `24b1ee6bd1d96f255889f167e59ef9c9399a6305`
- Substrate: `4ad76dc01fb94eb5ba1fa6779af893e3675cbad2`

## Contribute
If you'd like to contribute in any way, such as running validator nodes, feel free to do so.

## Composable Chains
To test cross-chain token transfers, please refer to this [guide](https://wiki.acala.network/build/development-guide/composable-chains).

# Collators

- Acala Mandala PC2: [wss://rococo-community-acala.laminar.codes/ws](https://polkadot.js.org/apps/?rpc=wss://rococo-community-acala.laminar.codes/ws)
  - Note: Please add our custom types in [./acala-types.json](./acala-types.json)
- Laminar Turbulence PC2: [wss://rococo-community-laminar.laminar.codes/ws](https://polkadot.js.org/apps/?rpc=wss://rococo-community-laminar.laminar.codes/ws)

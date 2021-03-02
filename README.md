# Community Rococo

This is an open community Rococo parachain testnet. The goal is to expedite parachain testing, and lower the overhead with shared infrastructure. 

# The Network
- Connect to Community-Rococo via [Polkadot-JS Web App](https://polkadot.js.org/apps/?rpc=wss%3A%2F%2Frococo-community.laminar.codes#/explorer).
- RPC endpoint: `wss://rococo-community.laminar.codes/ws`
- Bootnode: `/ip4/3.1.243.130/tcp/30335/p2p/12D3KooWDfjgSLT4bR535za1BZGSzCLdLgjhJz2s9tGQmnATmM8t`
- Chain spec: https://github.com/open-web3-stack/rococo-community/blob/master/rococo-community.json

## Run with Docker

```bash
docker run \
  -p 9944:9944 \
  -v $(pwd)/rococo-community.json:/rococo-community.json \
  parity/rococo:rococo-v1 --chain=/rococo-community.json \
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

- Polkadot: `9bc8915acd5507a77737371fdd892bb1f6a8db22`
- Cumulus: `fad35c28b1f73aaeb25dedb46674b48774c092b4`
- Substrate: `e03ca38d45f438932ec92bf69a40b6b16b6ec643`

## Contribute
If you'd like to contribute in any way, such as running validator nodes, feel free to do so. 

## Composable Chains
To test cross-chain token transfers, please refer to this [guide](https://wiki.acala.network/build/development-guide/composable-chains).

# Collators

- Acala Mandala PC2: `wss://rococo-community-acala.laminar.codes/ws`

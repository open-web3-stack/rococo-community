# rococo-community

## Network details

- RPC endpoint: wss://rococo-community.laminar.codes/ws
- Bootnode: /ip4/3.26.42.61/tcp/30333/p2p/12D3KooWA19bypiGn9aVaqNeBHmWqNobZQnRGk7dLRAQTvRPfgXy
- Chain spec: https://github.com/open-web3-stack/rococo-community/blob/master/rococo-community.json

## Run with docker

```bash
docker run \
  -p 9944:9944 \
  -v $(pwd)/rococo-community.json:/rococo-community.json \
  parity/rococo:rococo-v1 --chain=/rococo-community.json \
  --bootnodes=/ip4/3.26.42.61/tcp/30333/p2p/12D3KooWA19bypiGn9aVaqNeBHmWqNobZQnRGk7dLRAQTvRPfgXy \
  --ws-external \
  --rpc-cors=all \
  --rpc-methods=Unsafe \
  --wasm-execution=Compiled
```

# Faucet

Please post your details to https://github.com/open-web3-stack/rococo-community/discussions/2

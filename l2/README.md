# EigenLedger

We launch our network on [Layer 2 of Ethereum](https://github.com/ethereum-optimism/optimism), and extend the EVM and [solc](https://github.com/ieigen/solidity) to support privacy computing operators.


## [WIP] Add New Instructions for private computing

1. Hack solc;
```
git clone --recursive https://github.com/ethereum/solidity.git
cd solidity
git checkout 9e61f92bd

git apply add_instr.diff

./scripts/build_emscripten.sh
```

2. Update soljson.js

```
git clone https://github.com/offchainlabs/arbitrum.git
cd arbitrum/node_modules/solc/

# replace the soljson.js
./solcjs --bin hello.sol
```


# eth-deploy
This script should be used to deploy smart contracts on private ethereum blockchain.
It's using [embark](https://github.com/iurimatias/embark-framework).

### Requirements

Before using `eth-deploy` you need to install the following tools and you need to make sure that **ALL** of them are available in your PATH

- [node](https://nodejs.org/)
- [npm](https://www.npmjs.com/)
- [solc](https://github.com/ethereum/cpp-ethereum) *0.1.0, available as a part of cpp-ethereum --devel*
- [go-etheruem](https://github.com/ethereum/go-ethereum) *0.9.38*
- [embark](https://github.com/iurimatias/embark-framework) *0.5.0*

### usage

#### first time

```bash
# clone repository
git clone https://github.com/debris/eth-deploy
cd eth-deploy

# install dependencies
npm install

# start geth in background
# after that you should wait for DAG generation to complete
# and for few blocks to be mined
# the script will automatically stop minig when it has
# 'enought' ether
embark blockchain &

# deploy the contracts from contracts directory
# in the output you will see the addresses of deployed contracts
embark deploy         # deploy app/contracts/**/*.sol
```

#### without redeploying contracts

```bash
# just simply run
embark blockchain
```

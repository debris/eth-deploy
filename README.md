# eth-deploy
This script should be used to deploy smart contracts on ethereum blockchain.
It's using [embark](https://github.com/iurimatias/embark-framework).

### usage

```bash
git clone https://github.com/debris/eth-deploy
cd eth-deploy
npm install           # install dependencies
embark blockchain &   # start geth in background, you should wait few seconds after that
embark deploy         # deploy app/contracts/**/*.sol
```

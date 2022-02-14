# Solidity学習用
Solidity学習用レポジトリ。
こちらのhardhat + typescriptのテンプレートをもとに作成しています。
https://github.com/amanusk/hardhat-template

Solidityのバージョンは0.8.9にアップグレードして使っています。

## 内容
### TestToken.sol
ERC20トークン。テンプレートに入っていたものです。
### Artwork.sol
ERC721トークン。こちらを使用しています: [Create an NFT smart contract with HardHat](https://learn.figment.io/tutorials/create-nft-smart-contract-with-hardhat)

## Deploy
### ERC20
`npx hardhat run --network rinkeby ./scripts/deploy.ts`
### ERC721
`npx hardhat run --network rinkeby ./scripts/deploy-artwork.ts`

## Verify
アドレスは実際にデプロイされたアドレスに変更してください。
### ERC20
`npx hardhat verify --network rinkeby 0x509261ead018B9F86E7cbC39762eE44dF3d4C6A1`
### ERC721
`npx hardhat verify --network rinkeby 0x0CdD3298851fA01e555596A5d67E432D125ddE60 "Artwork Contract" "ART"`
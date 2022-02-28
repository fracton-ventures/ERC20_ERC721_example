# Solidity Tutorial No.1
A sample code for studying Solidity.
This sample code is made from the following hardhat + typescript template.
https://github.com/amanusk/hardhat-template

## Contents
### TestToken.sol
ERC20 token contract. This is included in the original template.
### Artwork.sol
ERC721 token contract. I picked up the following tutorial code: [Create an NFT smart contract with HardHat](https://learn.figment.io/tutorials/create-nft-smart-contract-with-hardhat)


## Preparation

### Nodejs & npm or yarn
To check nodejs version.
`node -v`
To check npm version.
`npm -v`

### Install packages
Run following command to install packages
`npm install`

### Check whether packages are installed successfully.
You can see hardhat options if they are installed successfully.
`npx hardhat`


## Test
Run following command to compile smart contracts.
`npx hardhat compile`

Run following command to export type.
`npx hardhat typechain`

Run following command to execute tests.
`npx hardhat test`


## Deploy
### ERC20
`npx hardhat run --network rinkeby ./scripts/deploy.ts`
### ERC721
`npx hardhat run --network rinkeby ./scripts/deploy-artwork.ts`

## Verify
Change the address to an actual deployed address.
### ERC20
`npx hardhat verify --network rinkeby 0x509261ead018B9F86E7cbC39762eE44dF3d4C6A1`
### ERC721
`npx hardhat verify --network rinkeby 0x0CdD3298851fA01e555596A5d67E432D125ddE60 "Artwork Contract" "ART"`
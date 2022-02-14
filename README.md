# Solidity Tutorial
A repo for studying Solidity.
This repo is made from the following hardhat + typescript template.
https://github.com/amanusk/hardhat-template

The solidity version is updated to 0.8.9 from the original version 0.6.*. 

## Contents
### TestToken.sol
ERC20 token contract. This is included in the original template.
### Artwork.sol
ERC721 token contract. I picked up the following tutorial code: [Create an NFT smart contract with HardHat](https://learn.figment.io/tutorials/create-nft-smart-contract-with-hardhat)

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
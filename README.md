# Polygon-Advanced-Module-1: Deploying Cross-Chain NFT Collection
## Project Overview:
Welcome to Polygon-Advanced-Module-1.This project focuses on deploying an NFT collection onto the Ethereum blockchain, followed by mapping the collection onto the Polygon network.

Additionally it involves transferring assets using the Polygon Bridge.

# Getting Started:
To begin, follow these steps:

. Download the entire repository to access all project contents.
.Navigate to the "Poly_Proof" project directory and install dependencies using the command:
-Copy code
-npm install
.Once dependencies are installed, run the test file using:
-bash
-Copy code
-npx hardhat test
.Deploying the ERC721 Contract:
-Before deployment, remember to rename ".env.example" to ".env" and provide your wallet's private key in the designated field (replace 'your wallet private key').
.To deploy the ERC721 contract to the Goerli Ethereum Testnet, use the following command:

## arduino
.Copy code
.npx hardhat run scripts/deploy.js --network goerli
#### Note: Upon deployment, an address will be generated. Copy this address into "contractAddress.js" (located in the metadata folder) and also in "batchMint.js" (located in the scripts folder).

#### Batch Minting NFTs:
Batch-mint NFTs using the deployed ERC721 contract with the command:

## arduino
.Copy code
.npx hardhat run scripts/batchMint.js --network goerli
.This script will mint the specified number of NFTs and associate them with your address.

#### Approve and Deposit NFTs to Polygon Mumbai:
To authorize and deposit the minted NFTs from Ethereum to the Polygon Mumbai network via the FxPortal Bridge, execute the following commands:

-arduino
-Copy code
-npx hardhat run scripts/approveDeposit.js --network goerli
# Author:
Project by Sourav Kashyap

# License:
This project is covered by the MIT License. 


# Final project – Solar Panel Purchase Receipt as an NFT

Before this class, I did not know JavaScript. So I learned JavaScript in August. Then, I realized that I did not know React. So I learned React in October. Still, I bit off way more than I could chew. So, so I present a simple NFT minter, where I, the smart contract deployer, am pretending to be a solar panel salesman who will store the receipts of solar panels I sell as NFTs. The NFTs contain metadata that will confirm the model of the solar panel sold; either a 400 watt model or a 440W model. Plus, that metadata has a URL to a PDF datasheet of each solar panel model. 

I’m also confident that, while my tests are failing, that this project demonstrates the application fo the concepts and best practices taught during this blockchain developer’s course. So, while I may fall short of the requirements of the final project, this course has been invaluable for me to pivot form some who has never coded before to someone who could honestly say that he used this pandemic to become a coding hobbyist.

I look forward to continue mastering JavaScript, Solidity and other languages in 2022.

## Deployed version url: ______________________

https://final-project-lvertiz.vercel.app

## How to run this project locally:

### Prerequisites

- Node.js >= v14
- Truffle and Ganache

## Directory structure

- Build folder: Artifacts of compiled solidity files, as JSON files. Files will appear in ‘contracts’ sub-folder after the solidity file is compiled
- Frontend Folder: Project's HTML frontend, and a JavaScript file to connect frontend to smart contract using Metamask as the service provider to the Ethereum Ropsten test network
- Contracts folder: Smart contracts for my NFT minter program that is deployed in the Ropsten testnet
- Migrations: Migration files for deploying contracts in Contracts directory. 
	
- Test: Tests for smart contracts. My testing file is a test written in Javascript, in my attempt to simulate interacting with my deployed contracts from ‘the outside world’ (i.e. via my dapp)


### Frontend

- Go to the code editor of your choice and open up the HTML file in the ‘Frontend’ folder
- Make surey our editor has ‘Live-Server’ installed. (I use Atom. Follow this link to install that package: https://atom.io/packages/atom-live-server)
- Run ‘Liver-Server’ on your code editor
- If your web browser does not open up a new window or tab automatically, open a new window or tab with the URL`http://localhost:3000`

## Public Ethereum wallet for certification:

`0x45FEB4865F00e359156A4F873C9Eef893b4191e7`


## Simple workflow using Front End

1. Run frontend website via Live-Server, or connect via public-facing URL
2. Connect and login with Metamask
3. Select solar panel model to mint an NFT receipt for (smart contract call)
4. Receive tokenId
5. Use tokenId to look up metadata in order to confirm model of the solar panel captured in the NFT/receipt


## Environment variables (not needed for running project locally)

```
ROPSTEN_INFURA_PROJECT_ID=
ROPSTEN_MNEMONIC=
```

## TODO features and workflows I wish I had been able to implement (but that I will tinker with in January 2022)

1)  Offering price for each solar panel in ETH; confirming user has sufficient funds in their wallet to pay for the product and transaction gas fees
2)  Remove onlyOwner modifier to use ERC721PresetMinterPauserAutoId.sol in order to:
	1) allow user to purchase a solar panel (i.e. mint an NFT) 
	2) Allow the front end to transfer the NFT to their user’s wallet address
	3) Allow the contract deployer (i.e me, the contract deployer) to collect the total amount of ETH used to pay for various transactions from various users
3)  Create a function/React component where, if the user does not have sufficient funds in their wallet to purchase a Solar Panel, they could be lead to a DeFi lender to procure a loan (or even a flash loan, perhaps) to obtain sufficient funding needed to pay for the solar panel purchase transaction.
![image](https://user-images.githubusercontent.com/69656638/144090678-435808a7-cf3e-4eef-b53f-170eedf35db3.png)

---
title: "Carbon Credits"
date: 2025-01-28
draft: false
heroStyle: big
summary: "Blockchain based carbon market"
tags: ["Project", "Blockchain", "Web Dev", "Web3"]
---
View the demo app [here](https://carbon-credit-sepolia.vercel.app/home)<br>
View the github source [here](https://github.com/devansh-srv/Carbon-Credit)

## Motivation

Main idea for this was to allow Corporations to fulfill thier CSR (Corporate Social Responsibily) by buying '*carbon credits*' from NGOs while also resolving some of the issues with traditional carbon markets such as corruption, double spending, lack of transperency etc. 

Using blockchain and web3 many of these issues can be resolved to finally use carbon markets for thier inteded purpose. It will not only help Corporations fulfill thier CSR but also prevent them from *'greenwashing'* all the while ensuring NGOs get proper funding

## History
Carbon trading originated in the 1990s as a market-based solution to combat climate change, starting with the Kyoto Protocol in 1997, which introduced emissions trading among countries. It later evolved into voluntary markets and cap-and-trade systems, allowing companies to trade carbon credits globally.
![Alt text](/projects/carbon_credits/International_Conference_Center_Kyoto.jpg "International Conference Center Kyoto")

## How it works
1. NGOs will register on the platform and create Carbon Credits based on thier projects which will then be put up for sale.
2. Companies or traders can buy these can buy these credits from the NGO and resell them further if they wish to.
   - For every resell of a carbon credit, 10% of the transaction value is returned to the original creator of the credit (NGO).
   - This mechanism ensures continuous funding support for the NGO's environmental projects.

3. Credits must be available for finite amount of time to prevent double spending, once the project is completed the credits will be expired and can’t be sold further.

4. Once the NGO completes the promised project, it can expire all credits associated with that project.
   - Once the NGO completes the promised project, it can expire all credits associated with that project.
   - The web app generates a certificate verifying the credit purchase and acknowledging the person’s contribution to offsetting specific amount of carbon.

## Technologies Used
### Smart contract
- Solidity: To write smart contracts
- Hardhat: For testing and deployment
- Metamask: To handle wallet and transactions

### Front-end
- React: To make web app
- EthersJS: To connect to front-end to smart contract

### Back-end
- Python/Flask: To write the server logic and apis
- PostgreSQL: Database
- Neon: To host the database

## Deployment
The smartcontract is deployed in Sepolia Testnet (view on [Etherscan](https://sepolia.etherscan.io/address/0x5E5D1D1Dc0EDDB4f9e9E05FD872642Cd78F6eF51)) at the address `0x5E5D1D1Dc0EDDB4f9e9E05FD872642Cd78F6eF51`

The front-end of the webapp was deployed on [vercel](https://www.vercel.com) and the backend was deployed on [render](https://www.render.com)

You can checkout the deployed app [here](https://carbon-credit-sepolia.vercel.app/home)

![Alt text](/projects/carbon_credits/deployed.png "[Deployed App](https://carbon-credit-sepolia.vercel.app/home)")


## Critism and Problems
While traditional carbon markets post a lots of problems which leads some people to believe that carbon markets have done more harm than good and I personally don't dissagree with this statement let me explain why.

There are two types of carbon market: **Cap-and-Trade** and **Carbon Offset**.

Cap-and-Trade works between companies each company has a cap on how much greenhouse gases it can emit in one year. Suppose Company A exceeded this limit while company B emitted below its cap. B will recieve allowance in form of *carbon credits* which it can then sell to A so that A can also meet the cap requirements.<br>This method recieves criticism for promting companies to just buy off thier carbon emissions instead of moving towards reductions.

In carbon offset method, this is the method we base our project on, there need to be net reductions, for example when projects that help reduce carbon (like renewable energy and reforestation) will recieve credits from thier carbon reductions (1 credit for 1 ton of CO2 reduced) and then they can sell it to corporations which then can claim carbon reductions based on this. The problem that arises with this is that shell companies pop up which claim  net carbon reduction through at best sketchy documentations. Famous example of this is JPMorgan, Disney buying carbon credits from [The Nature Conservancy](https://www.nature.org/en-us/) which issued carbon credits by saving forests that were never at risk read more about it here: [Bloomberg](https://www.bloomberg.com/features/2020-nature-conservancy-carbon-offsets-trees/)

This case highlights how easily carbon credits can be abused.

## Closing remarks
While a blockchain solution will not solve all the problems with carbon markets it can certainly reduce them by using a decentralised verfication method for credit issue can reduce chance of corruption and being immutable will rule out chance of cheating and double speding. Aditionally we could utilize digitally signed IOT devices to efficiently estimate carbon reduction.

Have a nice day !

### Image Credits
Feature image by [Maxim Tolchinskiy](https://unsplash.com/@shaikhulud) on Unsplash
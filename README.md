# WavePortal Project

## Introduction

WavePortal is a decentralized blockchain application where users can send a message by "waving" at the application. Each wave is stored on the Ethereum blockchain using a smart contract as the backend. When a user waves, they have a chance to win a prize in ether (ETH) if the random number generated is below a certain threshold.

## Live Link

[WavePortal Live](waveportal-14268.web.app/)

## Smart Contract

The smart contract code can be found on GitHub: [Smart Contract Code](https://github.com/kunal232i/smart_contract_waveportal/)

The smart contract is written in Solidity and deployed on the public Ethereum blockchain. It keeps track of the total number of waves, each wave's sender address, timestamp, and message.

**Important Note:** The keys and secret keys used for the application have been hidden in environment variables to ensure security.

## How to Run the Code

### Prerequisites

1. **Metamask:** Make sure you have the Metamask browser extension installed.
2. **Firebase Account:** To use the Firebase services for the frontend, you need a Firebase account and project set up.

### Steps to Run

1. Clone the GitHub repository containing the front-end code.
2. Set up your Firebase project and replace the `firebaseConfig` object in the `App.js` file with your Firebase configuration.
3. Install the required dependencies using `npm install`.
4. Deploy the smart contract on the Ethereum blockchain. You can use Remix, Truffle, or other tools for deployment. Note down the contract address and ABI.
5. Replace the `contractAddress` and `contractABI` variables in the `App.js` file with the deployed contract's address and ABI.
6. Start the development server with `npm start`.
7. Visit the application in your browser at `http://localhost:3000`.
8. Connect your wallet (Metamask) to the application to interact with the smart contract and wave messages.
9. Enter a message and click on the "Wave at Me" button to send a wave.
10. You may receive a prize in ether if the random number generated is below the threshold (50).

**Important Note:** Ensure you are on the Rinkeby or any other supported Ethereum testnet in Metamask to interact with the deployed smart contract. Also, make sure you have enough test Ether in your wallet to cover the gas fees.

## Frontend

The frontend is built using React and connects to the Ethereum blockchain via Metamask. Users can connect their wallet, wave messages, and view all the waves sent by various users.

Thank you for using WavePortal! Happy waving! 🌊👋

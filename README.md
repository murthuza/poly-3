<<<<<<< HEAD
<<<<<<< HEAD
# Polygon Advanced Module 3 Project: zkSNARK Circuit Implementation

## Description
This project aims to design and deploy a new zkSNARK circuit that implements specific logical operations using the circom programming language. You will create the circuit, deploy a verifier on-chain to verify the proofs generated from this circuit, and then deploy it on the Sepolia testnet.

## Prerequisites
- Node.js and npm installed
- Hardhat installed
- Sepolia testnet

## Steps

### 1. Clone the Project
Clone the repository using the following command:
```sh
git clone <repository_url>
```

### 2. Install Necessary Packages
Navigate to the project directory and install the required packages:
```sh
npm install
```

### 3. Implement the Logic Gate
Navigate to the `circom` directory and make the necessary changes to implement the given logic gate in the circom file.

### 4. Configure Hardhat for Sepolia Testnet
Edit `hardhat.config.ts` to include the Sepolia testnet configuration:
```ts
import { HardhatUserConfig } from "hardhat/config";
import "@nomiclabs/hardhat-waffle";
import "@nomiclabs/hardhat-ethers";

const config: HardhatUserConfig = {
  solidity: "0.8.4",
  networks: {
    sepolia: {
      url: "https://rpc2.sepolia.org/", // Add your preferred RPC URL
      accounts: [process.env.PRIVATE_KEY], // Add your private key
    },
  },
};

export default config;
```
Ensure you have your private key stored in a `.env` file and loaded using `dotenv`:
```sh
PRIVATE_KEY=your_private_key
```
```ts
require('dotenv').config();
```

### 5. Compile the Circuit
Run the following command to compile the circuit:
```sh
npx hardhat circom
```

### 6. Deploy the Contract
Deploy the contract to the Sepolia testnet using:
```sh
npx hardhat run scripts/deploy.ts --network sepolia
```

### 7. Verifier Result
If all steps are followed correctly, you will get a contract address where it is deployed and the verifier result should be `true`.

## Output
- Contract Address: The address where the contract is deployed on the Sepolia testnet.
- Verifier Result: `true`

## Authors
Kankatala Hemanth 
[kankatalah1@gmail.com](mailto:kankatalah1@gmail.com)


---

By following these steps, you will successfully implement and deploy a zkSNARK circuit that performs the desired logical operations on the Polygon Sepolia testnet.
=======
# poly3
>>>>>>> d2a5559e8539f823bd4eb820f21fd27dcd4c576d
=======
# poly3
>>>>>>> d2a5559e8539f823bd4eb820f21fd27dcd4c576d

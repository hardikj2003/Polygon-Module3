# Polygon-Module3
In this project I have created a circuit using the circom programming language that implements the following logical gate:
The goal of the project is to prove that the inputs A=0 and B=1 yield a 0 output. 

# Installation
To get started with the project, follow these steps:

1. clone the hardhat-circom repository :
    `git clone https://github.com/gmchad/zardkat`
   
2. Install the required dependencies :
     `cd zardkat`
     `npm i`
   
4. Installing snarkjs :
   `npm install -g snarkjs`

# Implementation
1. Write the correct circuit.circom implementation.
2. Compile the circuit to generate circuit intermediaries
    `npx hardhat circom `
3. It will generate the LogicCircuitVerifier.sol contract.

# Deployment
`npx hardhat run scripts/deploy.ts --network mumbai`
This script does 4 things:
1. It deploys the LogicCircuitVerifier.sol contract.
2. Generates a proof from circuit intermediaries with `generateProof()`.
3. Generates calldata with `generateCallData()`.
4. Calls `verifyProof()` on the verifier contract with calldata.
5. Lastly, the asserted output should turn out to be  `TRUE`.

# Video Walkthrough
https://www.loom.com/share/0450e731e3f140109d0f18108ebe6e72?sid=1e92d712-98d2-4932-89f9-a745d3afe44f

# Author 
HARDIK JAIN :)

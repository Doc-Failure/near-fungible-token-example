# `Near Fungible Token Example`

# 📄 Introduction
In this repository we will show how to use OpenBlimp to create a Fungible Token for the Near Protocol.

# 📦 Installation

To run this project locally you need to follow the next steps:

## Prerequisites

1. Make sure you've installed [Node.js] ≥ 12 (we recommend use [nvm])
2. Make sure you've installed yarn: `npm install -g yarn`
3. Install dependencies: `yarn install`
4. Create a test near account [NEAR test account]
5. Install the NEAR CLI globally: [near-cli] is a command line interface (CLI) for interacting with the NEAR blockchain

   yarn install --global near-cli

## Configure your NEAR CLI

Configure your near-cli to authorize your test account recently created:

    near login

## Build and deploy a Fungible Token

1. Build the smart contract:
       `yarn build:release`
2. Deploy the local smart contract 
       ` near dev-deploy --wasmFile ./build/release/main.wasm --accountId  <Your Near Test Account Id>`
3. (Optional) In the `src/main/assembly/index.ts` file you can modify the function the function `ft_initialize` to replace the stub parameter with you own parameters.
      
4. Use near-cli to init your fungible Token     
       ` near call  <Your Contract Account> ft_init --account-id <Your Near Test Account Id>`
(In the scripts folder you can find some files with a lot of usefull command.)
   
5. Open your Near wallet and interact with your new Token.

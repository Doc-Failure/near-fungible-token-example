# `Near Fungible Token Example`

# 📄 Introduction

# 📦 Installation

To run this project locally you need to follow the next steps:

## Step 1: Prerequisites

1. Make sure you've installed [Node.js] ≥ 12 (we recommend use [nvm])
2. Make sure you've installed yarn: `npm install -g yarn`
3. Install dependencies: `yarn install`
4. Create a test near account [NEAR test account]
5. Install the NEAR CLI globally: [near-cli] is a command line interface (CLI) for interacting with the NEAR blockchain

   yarn install --global near-cli

## Step 2: Configure your NEAR CLI

Configure your near-cli to authorize your test account recently created:

    near login

## Step 3: Build and make a smart contract development deploy

Build the smart contract code and deploy the local development server: `yarn build:release` (see `package.json` for a full list of `scripts` you can run with `yarn`). This script return to you a provisional smart contract deployed (save it to use later). You can also follow the instructions on the folder _scripts_.

# 📑 Exploring the smart contract methods

The following commands allow you to interact with the smart contract methods using the NEAR CLI (for this you need to have a provisional smart contract deployed).

```

```

1. yarn build:rel
2. near deploy --wasmFile ./build/release/main.wasm --accountId 2.b) optional 4 update -> dev-1646132742949-24755372237025
3. near call dev-1646132742949-24755372237025 ft_metadata --account-id doc_failure.testnet

# Swisstronik-PERC-20

This repository contains a setup for deploying and interacting with a PERC-20 token on the Swisstronik testnet using Hardhat. The setup includes scripts for deploying the contract, minting tokens, and transferring tokens, utilizing encrypted transactions with Swisstronik.

## Prerequisites

Ensure you have the following installed:

- Node.js (version 14.x or later)
- npm (version 6.x or later)

## Faucet

https://faucet.testnet.swisstronik.com/

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/Kadafimuamar/Swisstronik_PERC20_Task_4.git
    cd Swisstronik_PERC20_Task_4
    ```

2. Run

    ```bash
    npm install --save-dev @nomicfoundation/hardhat-toolbox
    npm install dotenv
    npm install @swisstronik/utils
    npm install @openzeppelin/contracts
    ```

## Create File .env for Private Key (Keep Safe for this)

1. 

```bash
PRIVATE_KEY=YOUR-PRIVATE-KEY
```



## Running

1. Compile

```bash
 npx hardhat compile
```

2. Deploy Perc-20

```bash
npx hardhat run scripts/deploy.js --network swisstronik
```

3. Minting Perc-20

```bash
npx hardhat run scripts/mint.js --network swisstronik
```

4. Transfer Perc-20

```bash
npx hardhat run scripts/transfer.js --network swisstronik
```

Success TX will appear like this :
![Jepretan Layar 2024-07-29 pukul 02 16 15](https://github.com/user-attachments/assets/4d8715d7-9e60-4c68-ac02-1516cb93d25b)


Ensure your private key is kept secure.
The transfer.js script is set to transfer tokens to the address 0x16af037878a6cAce2Ea29d39A3757aC2F6F7aac1

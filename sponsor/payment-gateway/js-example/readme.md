# Js Example 
This repository contains a Js application demonstrating:
1. Payment Gateway manage the sponsor policy to sponsor any transaction that send BEP20 to them.
2. User send ERC20 token transfers to payment gateway without pay gas fee through paymaster.

## Quick Start

The example is performed on BSC testnet, please ensure you have some test ERC20 on BSC testnet. (You can get some 
from the official faucet)

1. Install the dependency.
    ```shell
    $ npm install
    ```

2. Edit the script.
   
    Open index.js and replace the following placeholders:
   - 'USER_PRIVATE_KEY' with the user's private key that will pay to the Payment Gateway.
   - 'TOKEN_CONTRACT_ADDRESS' with the address of the ERC20 token you want to send
   - 'PAYMENT_RECIPIENT_ADDRESS' with the receiver account of the payment link generated by Payment Gateway
   - 'TOKEN_CONTRACT_ADDRESS' with the ERC20 token that the Payment Gateway support.
   - 'SPONSOR_API_KEY' to the API key created by the Payment Gateway in the Nodereal MegaNode Console. create one 
     from [here](https://docs.nodereal.io/docs/meganode-paymaster-sponsor-guidelines) if you don't have it.
   - 'SPONSOR_POLICY_ID' to the policy ID created by the Payment Gateway on Meganode Paymaster, create one
     from [here](https://docs.nodereal.io/docs/meganode-paymaster-sponsor-guidelines) if you don't have it.

3. Run script
    ```shell
    $ npm start
    ```
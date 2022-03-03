## Development

### Contracts

In your terminal, go to the COINFLIP 2.0 repo and type:
`cd blockchain`
`npm install`

To deploy your smart-contracts:

- Run `truffle migrate --network <<network name here>>` to deploy to the network of your choice. So for Rinkeby, type `truffle migrate --network rinkeby`
- Replace the contract address in `client/constants`
- Replace the abi file in `client/abis/coinFlip.json`
- Make sure to fund the contract in both ETH and LINK ([Faucet for the Rinkeby network](https://Rinkeby.chain.link/))

### Client

Next, move back into the COINFLIP 2.0 repo (`cd ../`), then type:
`cd client`
`npm install`

### Config

On each deploy, make sure to:
- Change the `COINFLIP_ADDRESS` in `/client/constants.js` to your deployed contracts address
- Copy the new abi file into `/abis` folder
- Enable/disable, and update the suitable networks in `truffle-config.js`
- Get your mnemonic seed phrase add it to `blockchain/.secret`

## Use

You are now set to start your local server. Make sure you're still in `COINFLIP/client` and type:
 `npm start`

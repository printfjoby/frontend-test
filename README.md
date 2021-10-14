# Web3.js Frontend Dev Assignment
Assignment is to create simple Ethereum Dapp using `typescript` and `react.js` which allows users to check their Weenus Token balance and send some of it to another wallet.

Please use the xd file for reference, all timings for transitions can be found in the TEST.xd file.

Also attached is our current design system that will show the sizes, fonts and colours used for the components.


Please use tailwindcss as css framework

This has not yet been updated to reflect the design part of the test so please use the TEST.xd file and video as reference of what you are supposed to create.

### 1. Preparations
- Install and setup [MetaMask](https://metamask.io/download.html) extension to your browser.
- Switch your MetaMask network from Ethereum Mainnet to `Ropsten Test Network`.
- Retrieve some of rETH to your MetaMask address from [this faucet](https://faucet.dimensions.network).
- Add/Start tracking `Weenus Token` in your MetaMask wallet. Weenus Token address is [0x101848D5C5bBca18E6b4431eEdF6B95E9ADF82FA](https://ropsten.etherscan.io/address/0x101848D5C5bBca18E6b4431eEdF6B95E9ADF82FA#code)
- Try to deliver code even if it fails or is not finished.

### 2. Assignment

- Create react.js project.
- Ask user to connect to MetaMask wallet once app is loaded or by clicking some button (choose one).
- If user is not yet connected to metamask - show "connect to metamask" message and button to connect if you choose to implement it.
- If user is connected to metamask, using web3.js:
  * show connected user's rETH balance.
  * show connected user's Weenus Token balance.
  * add form with two inputs - amount and receiver address, submiting form should initiate token transfer from your metamask wallet to receiver wallet. You can use `0x0000000000000000000000000000000000000000` wallet as receivers.
  * show pending transaction hash when form is submitted.
- *Bonus points for updating user balance without refresh page.*
- *Bonus points for checking and updating transaction status (pending, completed, failed).*
- Provide your source code as github repository.


To work with Weenus Token you will need contract jsonInterface, it's added to this repository as [./WeenusTokenABI.json](./WeenusTokenABI.json)
Weenus Token contract address: `0x101848D5C5bBca18E6b4431eEdF6B95E9ADF82FA`

! Weenus Token balance is shown with 18 decimals (1000000000000000000 returned from contract is equal 1 Weenus Token you would see in your metamask wallet)

Additional weightage will be given for following the coding best practices and the time taken to complete the test will also be considered.
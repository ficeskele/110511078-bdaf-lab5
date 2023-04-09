# 110511078-bdaf-lab5

1. Develop an ERC20 token: 
    - 18 decimals.
    - Minting and burning capability with onlyOwner access control.
    - Ability to transfer ownership
2. Deploy your ERC20 token. Mint 1000 tokens (i.e. 1000 * 10^18 units) to yourself. **(Record the address of your own token)**
3. Go to Aave, lend ETH and borrow DAI out **(Record your Borrow transaction)**
    1. Go to AaveV3 Goerli: [https://staging.aave.com/?marketName=proto_goerli_v3](https://staging.aave.com/?marketName=proto_goerli_v3) 
    2. On the left, Supply 0.05 ETH.
    3. Borrow some DAI (50 or 100)
4. Go to Etherscan and get the address of the DAI **(Record the address of the DAI token)**
    - As this is a testnet, there are a lot of different versions of DAI, we’re going to use the one you borrowed out from Aave.
5. Go to UniswapV2 to create a new liquidity pair: [https://app.uniswap.org/#/pools/v2](https://app.uniswap.org/#/pools/v2) 
    - Make sure you are on Goerli testnet
    - “Add V2 Liquidity”
    - paste the address of your DAI token you have in one field (the ui should show you that you have some)
    - Paste the address of your own token in the other field
    - We can actually set the initial price of the token by determining the ratio between DAI and your token: let’s make your token worth 10 DAI by supplying 100 DAI to 10 of your token. (or 50 DAI to 5 of your token).
    - Approve DAI and your token to Uniswap, and hit the Supply button. (It will ask you to “Create pool and Supply”)
    - You will receive some pool tokens as per this transaction. Look at your address on Etherscan and determine the address of the token. **(Record the address of the pool token)**
    - Try [Swap](https://app.uniswap.org/#/swap), you should be able to swap your token to DAI now. Buy 0.001 of your token now. **(Record the transaction)**
6. Create a [Safe (Gnosis’s multiSig solution) on Goerli](https://app.safe.global/new-safe/create) **(Record the address of your Safe multiSig address)**
    - Have 2 owners in the Safe. You can use Metamask to generate the second address.
    - Set the Threshold as 2 out of 2 owners. This means that every time this multiSig is sending a transaction, both of these owners have to sign.
7. Transfer Ownership of your token to your Safe multiSig address. **(Record the transaction)**
8. Mint 10000 of your tokens by using your Safe multiSig address to your own address **(Record the transaction)**
9. Sell all of the 10000 tokens into the Uniswap pool you created. **(Record the transaction)**

---

Etherscan link to your token*

[https://goerli.etherscan.io/token/0xae79bac58e460a39addcf544a1f4e1af94e23d2f](https://goerli.etherscan.io/token/0xae79bac58e460a39addcf544a1f4e1af94e23d2f)

Etherscan link to Aave Borrow transaction *

[https://goerli.etherscan.io/tx/0x58498481dc4c69d7c4b7d9c81c6c0648b6c3a75550cf3a2a5032ecb50da7ec6f](https://goerli.etherscan.io/tx/0x58498481dc4c69d7c4b7d9c81c6c0648b6c3a75550cf3a2a5032ecb50da7ec6f)

Etherscan link to DAI token*

[https://goerli.etherscan.io/token/0xba8dced3512925e52fe67b1b5329187589072a55](https://goerli.etherscan.io/token/0xba8dced3512925e52fe67b1b5329187589072a55)

Etherscan link to UniswapV2 pool token*

[https://goerli.etherscan.io/token/0x4244150f1a015b62685248c933d6f25b622a671b](https://goerli.etherscan.io/token/0x4244150f1a015b62685248c933d6f25b622a671b)

Etherscan link to UniswapV2 transaction of buying token *

[https://goerli.etherscan.io/tx/0x9b5ff38124e22e707185ab4b1b422b2707f3ac11f32443da1ba40a18177b6f74](https://goerli.etherscan.io/tx/0x9b5ff38124e22e707185ab4b1b422b2707f3ac11f32443da1ba40a18177b6f74)

Etherscan link to Gnosis Safe multiSig*

[https://goerli.etherscan.io/address/0x2168504FAEd47ba7004D442D24ba0A8e4F9196f0](https://goerli.etherscan.io/address/0x2168504FAEd47ba7004D442D24ba0A8e4F9196f0)

Etherscan link to the transaction of Ownership transfer to Gnosis Safe*

[https://goerli.etherscan.io/tx/0xbae233b01a20414a82e1e6b68950a99bdb2f51884b0ff077fb1118b13d88eb79](https://goerli.etherscan.io/tx/0xbae233b01a20414a82e1e6b68950a99bdb2f51884b0ff077fb1118b13d88eb79)

Etherscan link to the transaction of minting tokens through Gnosis Safe*

[https://goerli.etherscan.io/tx/0xd68cad006ff7882ad04dbe0f5fcdda701abf3f0f21be29e4ba8f8fc823a92653](https://goerli.etherscan.io/tx/0xd68cad006ff7882ad04dbe0f5fcdda701abf3f0f21be29e4ba8f8fc823a92653)

Etherscan link to the transaction of selling the tokens*

[https://goerli.etherscan.io/tx/0xbf57208d5b94d34af6228eead93f817f9d7e1169fd9b8bb306b3e6519694de3a](https://goerli.etherscan.io/tx/0xbf57208d5b94d34af6228eead93f817f9d7e1169fd9b8bb306b3e6519694de3a)

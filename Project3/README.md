# NFT Marketplace - Lets Build a Rug Pull

## ART

1) To start with a collection, you need art. To make Art, its ideal to have a photo editor if you want it to be spiffy, otherwise, Powerpoint (PPT) is fine

Using a Photo Editor, we will need to create:
-PNG file(s) that are of our art
-Metadata file(s) that correspond to our art

2) Next, we will upload these files to IPFS (https://www.pinata.cloud)
3) Create a front end using:
-[Next.js](https://nextjs.org/) - to handle routing
-[Tailwindcss](https://tailwindcss.com/)

4) Create NFT Smart Contract on Rinkeby Testnet and integrate front end to communicate with NFT contract.

To Run this:
pip install react
npm install react react-dom
npm install merkletreejs keccak256 --force
npm install @alch/alchemy-web3 --force
npm i @nomiclabs/hardhat-etherscan --force

npx hardhat run scripts/deployContracts.js --network
npx hardhat compile
installs npm install hardhat ethers @nomiclabs/hardhat-waffle ethereum-waffle chai @nomiclabs/hardhat-ethers @openzeppelin/contracts dotenv

5) Compile the smart contract
Before compiliation:
- ensure whitelist addresseses are set
- ensure the .env file has the following:
    a) NEXT_PUBLIC_ALCHEMY_RPCURL=url of api setup with https://www.alchemy.com/
    b) NEXT_PUBLIC_FORMATIC_KEY
    c) NEXT_PUBLIC_DAPP_ID
    d) METAMASK_PRIVATE_KEY=<private key of meta maskwallet>
    e) ETHERSCAN_API_KEY
To compile and get the artifacts file:

 
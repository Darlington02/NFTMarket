# Starknet NFTMarketplace

NFTMarket is a simple Marketplace to buy and sell NFTS (ERC721) on StarkNet. The workflow is simple:
1. A seller lists his/her NFT on the marketplace.
2. A buyer comes along to purchase using ETH, depending on the NFT's listing price.
3. The user becomes the new owner of the NFT.

## Project Content
1. ERC721.cairo - Cairo contract for creating a simple ERC721 token using Openzeppelin's library.
2. market.cairo - Cairo contract for the NFT marketplace.
3. IERC721.cairo - Interface to interact with an ERC721 contract.
4. IERC20.cairo - Interface to interact with an ERC20 contract.

## Getting Started
1. Ensure to install Protostar following the [docs](https://docs.swmansion.com/protostar/docs/tutorials/installation). 
2. Clone the repository and try running `Protostar build`
3. The codes are properly commented for better readability.
4. To deploy a new ERC721 token on Goerli2:
```protostar deploy ./build/ERC721.json --gateway-url "https://alpha4-2.starknet.io" --chain-id 1536727068981429685321 --inputs 1443913798310970484084 5129805 0x046c5877EE8d297107Bd8E507Fb97b8cAB4ECD6C83892AD92EA40100412b4976```
5. To deploy the NFTMarket contract on Goerli2:
```protostar deploy ./build/market.json --gateway-url "https://alpha4-2.starknet.io" --chain-id 1536727068981429685321```

## Deployed Contracts
1. ERC721 - `0x02f5222bdb8e68b59736e1490c5ec36ab32f609e4e7058a4042841a51a6cec94`
2. NFTMarket - `0x05b3f40d5cdac77a4e922d8765a5a6ae96e64dc2a4796187d9a25166d0da2235`

Available tokens for sale:
1. Token ID - 2, Listing price 0.001ETH
2. Token ID - 3, Listing price 0.001ETH
3. Token ID - 4, Listing price 0.001ETH
4. Token ID - 5, Listing price 0.001ETH

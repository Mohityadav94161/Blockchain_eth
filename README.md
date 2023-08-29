# Genesis.json/Create your own Private Network in Ethereum 
 1. Install goethereum
 2. make a genesis block so for that lets make genesis.json file
 3. Below is file content

**{
  "config": {
    "chainId": 1267,   
    "homesteadBlock": 0,
    "eip150Block": 0,
    "eip155Block": 0,
    "eip158Block": 0,
    "byzantiumBlock": 0,
    "constantinopleBlock": 0,
    "petersburgBlock": 0,
    "istanbulBlock": 0
    
  },
  "difficulty": "0x400",
  "gasLimit": "0x80000000",
  "alloc": {
    "0x1AEFE3BAbe9a867333D39E0700d62B147cC00C10": {
      "balance": "100000000000000000000000000000000"   
    }
  },
  "coinbase": "0xc446F5042EB81b7ef79eB1368Fe2b3EF2a198b5C",
  "timestamp": "0x5C2D29D0",   
  "extraData": "",
  "mixHash": "0x0000000000000000000000000000000000000000000000000000000000000000",
  "nonce": "0x0"
}**

## config: This section defines network-specific configuration options.

## chainId:
An integer representing the chain ID for the network. It's a unique identifier for your network. For a private network, you can choose any number, but make sure it's distinct from Ethereum's mainnet and other testnets.
homesteadBlock, eip155Block, eip158Block, byzantiumBlock, constantinopleBlock, petersburgBlock, istanbulBlock: These parameters determine at which block numbers specific Ethereum improvement protocols (EIPs) should be activated. Setting them all to 0 means these protocols are active from the genesis block.
difficulty: A string representing the difficulty level for mining blocks. For a private network, you can typically set this to a low value, as mining will be easier compared to the main Ethereum network.

## gasLimit: 
A string indicating the maximum amount of gas that can be used in a block. This value affects the overall processing capacity of your network.

## alloc: 
This section defines initial account balances.

## YOUR_ACCOUNT_ADDRESS: 
Replace with an Ethereum address. This is the address of an account that will have an initial balance.
## balance: 
A string representing the initial balance of the account in wei (the smallest denomination of Ether).
coinbase: An Ethereum address that will receive mining rewards. This is the address that validates and mines new blocks.

## timestamp:
A hexadecimal representation of the timestamp for the genesis block. You can use online tools to convert a regular timestamp to hexadecimal.

## extraData: 
Additional data that can be included in the genesis block. This is usually left empty for a private network.

## mixHash: 
A hash used in Ethereum's proof-of-work algorithm. For a private network, this can be set to a predefined value.

## nonce: 
A random value used in Ethereum's proof-of-work algorithm. Similar to mixHash, you can set this to a predefined value for a private network.




# Genesis.json/Create your own Private Network in Ethereum 
 1. Install goethereum
 2. make a genesis block so for that lets make genesis.json file
 3. Below is file content

```{
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
}```

**alloc: A list of account addresses and their initial balance. These are the accounts that will have Ether initially.
coinbase: The address of the account that will receive mining rewards.
difficulty: The difficulty level for mining blocks.
gasLimit: The maximum amount of gas that can be used in a block.
timestamp: The timestamp for the genesis block.
config: Network-specific configuration options.
nonce: A random value used in the proof-of-work algorithm.**

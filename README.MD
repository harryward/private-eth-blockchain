
# Private Blockchain
#### by Harry Ward

Documentation
https://github.com/ethereum/go-ethereum/wiki/Private-network



### Init Geth with Genesis Block
To create a database that uses this genesis block, run the following command. This will import and set the canonical genesis block for your chain.

geth --datadir ./dataDir init genesis.json

### Server Startup
geth --datadir ./dataDir --networkid 15 --rpc --rpccorsdomain "*"  console 2>> geth.log

### Logging
tail -f geth.log
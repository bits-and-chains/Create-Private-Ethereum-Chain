### Creating Your Own Private Chain

__

#### Software Requirements

[Homebrew](http://brew.sh/)

[Ethereum](https://www.ethereum.org/)

[geth](https://github.com/ethereum/go-ethereum)



### Quick Start

Download Ethereum via Homebrew

Download geth

```
brew tap ethereum/ethereum
brew install ethereum

```


Start your private blockchain using geth


```
geth --identity "ExampleChain" --datadir --nodiscover --maxpeers 0 --rpc ~/.ethereum_private init genesis.json
```


### Notes and Definitions


```
geth --datadir ~/.ethereum_private init genesis.json
```
`geth`: the Go client

`genesis.json`: The location of your genesis file. Genesis file is like the config file for your blockchain. Some of the parameters you can set in the genesis file includes how much ether you would like to prepopulate in your blockchain. Genesis creates the first "block" in your private blockchain.

`maxpeers 0`: Makes the private node non-discoverable

`rpc`: Enables RPC interface on node

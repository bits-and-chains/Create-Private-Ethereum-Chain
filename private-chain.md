__Creating Your Own Private Chain__

(https://giphy.com/gifs/Nu9WW7RBM3Rle/html5)

_Note these intstructions are or a Mac but will have more intstructions for other platforms soon_

#### Software Requirments

[Homebrew](http://brew.sh/)
[Ethereum](https://www.ethereum.org/)




### Quick Start
1. Get some background information about terminals [here](ReadMe.md)
2. Open up a terminal
3. Download Ethereum via Homebrew:

```
brew tap ethereum/ethereum
brew install ethereum

```


4. Start your private blockchain using geth:


```
geth --datadir ~/.ethereum_private init ~/dev/genesis.json

geth --fast --cache 512 --ipcpath ~/Library/Ethereum/geth.ipc --networkid 1234 --datadir ~/.ethereum_private  console
```


### Notes and Definitions

Let's take a closer look at those parameterst sthat we typed in for #4

```
geth --datadir ~/.ethereum_private init ~/dev/genesis.json
```
`geth`: is the client

`--datadir ~/.ethereum_private`: the directory where you will keep your blockchain datadia

`~/dev/genesis.json`: The location of your genesis file. Genesis file is like the config file for your blockchain. Some of the parameters you can set in the genesis file includes how much ether you would like to prepopulate in your blockchain. Genesis creates the first "block" in your private blockchain.

`nonce`: 

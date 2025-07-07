## Foundry

**Foundry is a blazing fast, portable and modular toolkit for Ethereum application development written in Rust.**

Foundry consists of:

-   **Forge**: Ethereum testing framework (like Truffle, Hardhat and DappTools).
-   **Cast**: Swiss army knife for interacting with EVM smart contracts, sending transactions and getting chain data.
-   **Anvil**: Local Ethereum node, akin to Ganache, Hardhat Network.
-   **Chisel**: Fast, utilitarian, and verbose solidity REPL.

## Documentation

https://book.getfoundry.sh/

## Usage

### New Forge Project

```shell
$ forge init
```

### Build

```shell
$ forge build
```

### Test

```shell
$ forge test
```

### Format

```shell
$ forge fmt
```

### Gas Snapshots

```shell
$ forge snapshot
```

### Anvil

```shell
$ anvil
```

### Deploy

```shell
$ forge script script/Counter.s.sol:CounterScript --rpc-url <your_rpc_url> --private-key <your_private_key>
```

### Cast

```shell
$ cast <subcommand>
```

### Help

```shell
$ forge --help
$ anvil --help
$ cast --help
```
Ethereum Improvement Proposals (EIP)
https://eips.ethereum.org/erc

Go through the methods of ERC-20
https://eips.ethereum.org/EIPS/eip-20

## Create Token from imports

Go to Openzepplin
https://docs.openzeppelin.com/contracts/5.x/

Install OpenZepplin
https://github.com/OpenZeppelin/openzeppelin-contracts


```shell
$ forge install openZeppelin/openzeppelin-contracts@v5.0.2
```
Or 


```shell
$ forge install openZeppelin/Openzeppelin-contracts
```
Now we can see ERC20.sol here
(lib/openzeppelin-contracts/contracts/token/ERC20/ERC20.sol)


Another repository is Solmate

https://github.com/transmissions11/solmate

Then do remappings in foundry.toml

Get the Makefile from https://github.com/Cyfrin/foundry-erc20-cu/blob/main/Makefile

```shell
$ make anvil
```
Create another terminal and run deploy command

```shell
$ make deploy
```
Now the Token has been depoyed to the anvil chain









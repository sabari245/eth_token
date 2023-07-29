# ETHToken

ETHToken is a simple token contract that allows users to mint and burn tokens. It is written in Solidity 0.8.0 and follows the MIT license.

## Features

- The contract has public variables that store the details about the token, such as its name, abbreviation, and total supply.
- The contract has a mapping of addresses to balances, which tracks how many tokens each account owns.
- The contract has a mint function that takes an address and a value as parameters. The function increases the total supply by that value and increases the balance of the given address by that amount.
- The contract has a burn function that works the opposite of the mint function. It takes an address and a value as parameters and reduces the total supply and the balance of the given address by that amount. The function also checks that the balance of the address is greater than or equal to the value to be burned.

## Usage

To use this contract, you need to have a Solidity compiler and a web3 provider. You can deploy the contract using Remix or Truffle. You can also interact with the contract using web3.js or web3.py.

To mint tokens, you need to call the mint function with an address and a value. For example, if you want to mint 100 tokens for account 0x1234, you can do:

```solidity
myToken.mint(0x1234, 100);
```

To burn tokens, you need to call the burn function with an address and a value. For example, if you want to burn 50 tokens from account 0x1234, you can do:

```solidity
myToken.burn(0x1234, 50);
```

To check the balance of an account, you can use the balances mapping. For example, if you want to check the balance of account 0x1234, you can do:

```solidity
myToken.balances(0x1234);
```

To check the total supply of tokens, you can use the totalSupply variable. For example, if you want to check the total supply of tokens, you can do:

```solidity
myToken.totalSupply();
```


# Token Solidity Contract

This Solidity contract implements a simple token with functionalities to mint and burn tokens.

## Overview

This contract includes the following functionalities:

1. **Public Variables:**
   - `tName`: Token name.
   - `tAbbrv`: Token abbreviation.
   - `t_supply`: Total token supply.

2. **Mapping:**
   - `balance`: Maps addresses to token balances.The second mapping is {balance{, which associates addresses with token balances.

3. **Mint Function:**
   - Adds a certain amount to the overall supply.
   - Adds that amount to the balance of a given address.

4. **Burn Function:**
   -Reduces the overall supply by a given amount.
   -If there is enough money in the designated address, it reduces the balance by that amount.

## Usage

To interact with this contract, you can follow these steps:

1. **Deploy Contract:** - Set up the contract on an Ethereum blockchain network that is compatible.

2. **Mint Tokens:** - Tokens can be created by using the `mint` function.
   Give the required value to be minted along with the address where the tokens will be produced.

3. **Burn Token** -Existing tokens can be destroyed by using the burn function.
Give the desired burn value and the address from which the tokens will be burned.

## Example

```solidity
// Deploy the contract
MyToken tokenContract = new MyToken();

// Mint tokens
tokenContract.mint(addressToMint, valueToMint);

// Burn tokens
tokenContract.burn(addressToBurn, valueToBurn);
```

## License

This contract is released under the [MIT License](LICENSE).


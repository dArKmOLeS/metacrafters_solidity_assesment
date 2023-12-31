# metacrafters_solidity_assesment
MYTOKEN
----------------------------------
This is a simple token contract created in Solidity. The contract allows the user to create and destroy tokens with the help of mint() and burn(), as well as storing information about the token and balance as well.

Requirements-
----------------------------------
The contract has public variables that store the details about the coin:

tokenName: A string representing the name of the token.
abbrv: A string representing the abbreviation of the token.
totalSupply: An unsigned integer representing the total supply of the token.
The contract has a mapping of addresses to balances:

balances: A mapping that associates addresses with their corresponding token balances.
The contract has a mint function that increases the total supply and the balance of the "sender" address by a given value:

Parameters-
-----------------------------------
_address: The address where the tokens will be sent after they have been created.
_value: The quantity of tokens that will be produced.
Increase the totalSupply by the specified amount.
The balance of the _address should be raised by _value.
The contract has a burn function that subtracts a specified amount from both the balance at the "sender" address and the total supply:

Parameters-
----------------------------------
_address: The address from which the tokens will be burned.
_value: The amount of tokens to be burned.
Actions:
Check if the balance of the _address is greater than or equal to _value.
If true, decrease the totalSupply by _value.
Decrease the balance of the _address by _value.

Usage-
----------------------------------
Deploy the MyToken contract on an Ethereum network that is supported.

When the contract is deployed, you can communicate with it by calling the following functions:

mint: Produces fresh tokens and sends them to a given address.

I have used Remix, an online solidity IDE , https://remix.ethereum.org/

Parameters-
-------------------------------------
_address: The address to which the tokens will be minted.
_value: The amount of tokens to be minted.
burn: Destroys existing tokens by reducing the total supply and the balance of a specified address.

Parameters-
----------------------------------------
_address: The address from which the tokens will be burned.
_value: The amount of tokens to be burned.
License
This contract is licensed under the MIT License. SPDX-License-Identifier: MIT.

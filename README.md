# MyToken Smart Contract
The MyToken smart contract is an ERC-20-like token deployed on the Ethereum blockchain. It defines basic functionalities for minting, burning, and managing balances. This implementation uses Solidity version 0.8.18 and comes with the MIT license.

# Features
Name: "Nikita"
Symbol: "NK"
Total Supply: Dynamic, initially set to 0, and increases with minting and decreases with burning.
Minting: Allows the creation of new tokens by increasing the total supply and updating the balance of a specified address.
Burning: Allows the destruction of tokens by decreasing the total supply and updating the balance of a specified address.

## Public Variables
string public name: The name of the token ("Nikita").
string public symbol: The symbol representing the token ("NK").
uint public totalSupply: The total number of tokens in circulation (initially 0).

## Mappings
mapping(address => uint) public balances: A mapping that holds the token balance for each address.

## Functions
1. mint(address _address, uint _value)
Increases the total supply by _value.
Adds _value to the balance of the address _address.

## Parameters:
_address: The address to which new tokens will be minted.
_value: The amount of tokens to mint.
2. burn(address _address, uint _value)
Decreases the total supply by _value.
Reduces the balance of the address _address by _value, if the balance is sufficient.

## Parameters:
_address: The address from which tokens will be burned.
_value: The amount of tokens to burn.

## Usage
* Minting: To mint new tokens, call the mint function with the recipient's address and the number of tokens to create. This increases the total supply and updates the recipient's balance.
```
mint(0xRecipientAddress, 100);
```
* Burning: To burn tokens, call the burn function with the address holding the tokens and the number of tokens to destroy. This decreases the total supply and updates the balance.
```
burn(0xTokenHolderAddress, 50);
```
# License
This project is under MIT license.

# Contact details
Gmail : yadavnikita119@gmail.com
Name : Nikita Yadav

# EgoToken Smart contract

`EgoToken` is an ERC-20 token named "EGO" with the symbol "ego" deployed on the Avalanche Fuji Testnet. This token allows the owner to mint new tokens, create items associated with unique IDs, burn tokens, and redeem items. The contract is built on the Ethereum blockchain using OpenZeppelin's ERC-20 implementation.

# Contract Information

Functions

- ## Constructor:

 Initializes the ERC-20 token with the specified name and symbol.
 Sets the contract deployer as the owner.

- ## mint(address to, uint256 amount):

Mints new tokens and assigns them to the specified address.
Only the contract owner can call this function.

- ## createItems(string memory _name, uint256 amount):
  
Creates items associated with unique IDs.
Only the contract owner can call this function.

- ## burn(uint amount):
       
 Burns a specified amount of tokens from the caller's balance.
Ensures that the caller has a sufficient balance to burn.

- ## redeem(uint8 itemID_):
       
 Redeems items associated with a given item ID.
Transfers the ownership of the item to the caller.

- ## viewItemOwner(uint8 itemID_):
       
 Returns the current owner of the item associated with the given item ID.

- ## showItem(uint id_):
       
 Returns detailed information about the item associated with the given ID.


# Deployment

Deployment on Avalanche Fuji Testnet: 

Contract Address : 0xF6dB22642Bf6dAC8c540260A2A11C4C7e69Ca653

https://testnet.snowtrace.io/address/0xf6db22642bf6dac8c540260a2a11c4c7e69ca653



## Contract Interactio: 

- The contract owner can mint new tokens and create items using the respective functions.

- Any address with a balance can burn their tokens.
    
- Items can be redeemed by calling the redeem function, and their ownership can be viewed using the viewItemOwner function.
- Detailed information about items can be obtained using the showItem function.



## Authors
[@metacraftersio]()

[Oche Esther](https://twitter.com/Estheroche1)

## License

This project is licensed under the MIT License - see the LICENSE.md file for details.
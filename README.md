# ERC20 token
# Overview
The AasthaToken smart contract is an ERC-20 compatible token implemented in Solidity. It provides basic functionalities for minting, burning, and transferring tokens. The contract is named "AasthaToken" with the symbol "Abc" and has a fixed initial supply that can be expanded by the owner.

# Features
Token Details: Stores token name, symbol, decimals, and total supply.
Ownership: Restricts certain functions to be accessible only by the contract owner.
Minting: Allows the contract owner to mint new tokens.
Burning: Allows any token holder to burn their tokens.
Transferring: Allows token holders to transfer tokens to others.
# Contract Details
# State Variables
name: The name of the token (AasthaToken).
symbol: The symbol of the token (Abc).
decimals: The number of decimals the token uses (1).
totalSupply: The total supply of tokens.
balanceOf: A mapping of addresses to their respective token balances.
owner: The address of the contract owner.
# Events
Transfer: Emitted when tokens are transferred from one address to another.
Mint: Emitted when new tokens are minted.
# Constructor
The constructor initializes the token with the following:

Sets the token name, symbol, and decimals.
Mints an initial supply of 100 tokens to the contract owner.
Sets the deployer of the contract as the owner.
# Modifiers
onlyOwner: Restricts the execution of certain functions to the contract owner.
# Functions
mint_Tokens(address To, uint256 Amount) internal
Mints new tokens and assigns them to the specified address.

# Parameters:
To: The address to receive the minted tokens.
Amount: The number of tokens to mint.
Emits:
Mint
# Transfer
mint(address To, uint256 Amount) public onlyOwner
Public function that allows the contract owner to mint new tokens.

# Parameters:
To: The address to receive the minted tokens.
Amount: The number of tokens to mint.
# Calls:
mint_Tokens
burn(uint256 Amount) public
Allows token holders to burn a specific amount of their tokens.

# Parameters:
Amount: The number of tokens to burn.
Emits:
Transfer
transfer(address To, uint256 Amount) public
Allows token holders to transfer tokens to another address.

Parameters:
To: The address to receive the tokens.
Amount: The number of tokens to transfer.
Emits:
Transfer
# Usage
Deployment: Deploy the contract on the Ethereum blockchain. The deployer will be the initial owner and will receive the initial supply of tokens.
Minting: The owner can mint additional tokens using the mint function.
Burning: Any token holder can burn their tokens using the burn function.
Transferring: Token holders can transfer their tokens to others using the transfer function.
# License
This contract is licensed under the MIT License.

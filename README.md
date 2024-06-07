This Token contract is an Ethereum smart contract written in Solidity. It implements a basic ERC20 token with features such as token transfers, token minting, and token burning. Additionally, it includes functionality to pause token transfers and transfer ownership of the contract.

# Overview
Name: AasthaToken
Decimals: 1
Total Supply: 40,000
Owner: The deployer of the contract
# Features
Token Metadata: The contract defines the token name, decimals, and total supply.
Token Balances: The contract keeps track of the token balances of all addresses.
Events: The contract emits events for token transfers, minting, ownership transfer, pause, and unpause actions.
Owner Management: The contract allows the owner to transfer ownership to another address.
Pause Functionality: The contract includes a pause mechanism to temporarily stop token transfers.
Token Minting: The owner can mint new tokens and allocate them to any address.
Token Burning: Token holders can burn their own tokens to reduce the total supply.
# Functions
mint: Allows the owner to mint new tokens and assign them to a specified address.
burn: Allows token holders to burn their own tokens, reducing the total supply.
transfer: Allows token holders to transfer tokens to other addresses.
transferOwnership: Allows the owner to transfer ownership of the contract to another address.
pause: Allows the owner to pause token transfers temporarily.
unpause: Allows the owner to resume token transfers after pausing.
# Usage
Deployment: Deploy the contract to an Ethereum-compatible blockchain network.
Initialization: Upon deployment, the contract initializes with the specified token parameters and initial supply.
Token Management: The owner can manage the token by minting new tokens, burning tokens, transferring ownership, pausing, and unpausing token transfers.
Token Interaction: Token holders can transfer tokens to other addresses using the transfer function.
Event Monitoring: Monitor emitted events for token transfers, minting, ownership transfer, pause, and unpause actions.
# Security Considerations
Ownership: Exercise caution when transferring ownership as the new owner gains control over the contract.
Pause Mechanism: Use the pause functionality responsibly to prevent unintended consequences such as frozen tokens.
Token Burning: Ensure that token burning actions are performed by authorized holders to prevent loss of tokens.

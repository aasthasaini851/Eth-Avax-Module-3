# Aastha Token Smart Contract
This repository contains the Solidity code for the Aastha Token (ABC), a simple ERC20-like token with minting, burning, and transfer functionalities.

# Contract Overview
The Aastha contract implements a basic token with the following features:

Minting: The ability to create new tokens and add them to a specified address.
Burning: The ability to destroy tokens from a specified address.
Transfer: The ability to transfer tokens from one address to another.
# Functions
# mint(address to, uint256 amount)
Mints new tokens and assigns them to the specified address.

to: The address that will receive the new tokens.
amount: The number of tokens to mint.
# burn(address from, uint amount)
Burns a specified number of tokens from the specified address.

from: The address from which tokens will be burned.
amount: The number of tokens to burn.
# transfer(address from, address receiver, uint256 amount)
Transfers a specified number of tokens from one address to another.

from: The address from which tokens will be transferred.
receiver: The address that will receive the tokens.
amount: The number of tokens to transfer.
# Deployment
To deploy this contract, follow these steps:

Open Remix IDE.
Create a new file and paste the contract code into it.
Ensure you have the correct import statement and that Remix can fetch the dependencies.
Compile the contract using the appropriate Solidity compiler version (at least 0.8.0).
Deploy the contract using the "Deploy & Run Transactions" tab.

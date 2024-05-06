# Solidity Functions and Errors

Overview 

This is a simple Ethereum smart contract written in Solidity that allows users to withdraw, deposit, and check their balance. It demonstrates the use of  require(), revert(), and assert() statements for error handling and validation.

## Requirements
To interact with the smart contract, you'll need:
* A development environment for Ethereum smart contracts
* An Ethereum wallet or client (e.g., MetaMask) to compile,deploy and interact with the smart contract.

## Authors
David Joshua B. Bucol

## Smart Contract Details 
The smart contract `MyContract` includes the following functions:

### `deposit(address _address, uint _value)`
This function allows users to deposit funds into their account. It checks if the deposit value is greater than 100 using the `require()` statement. Funds are then added to the user's balance. Subsequently, the `assert()` statement verifies that the balance has indeed increased by the deposited amount. If not, it reverts the transaction with an error message.

### `withdraw(address _address, uint _value)`
Users can withdraw funds from their account using this function. It verifies if the user has sufficient balance using `require()`. Upon successful validation, the specified amount is deducted from the user's balance. Similar to the `deposit` function, the `assert()` statement ensures the balance remains non-negative after the withdrawal. If it fails, the transaction is reverted with an appropriate error message.


## License
This project is licensed under the MIT License - see the LICENSE.md file for details

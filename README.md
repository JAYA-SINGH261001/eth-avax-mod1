# Eth-avax-mod1
# Error Handling in Solidity 
This Solidity program is a simple program which shows the functioning of the assert , require and revert fuctiona and their importance in the program. The contract includes a function callled "Error" that helps the sender or the owner to find the speed of the given distance. Let's explore the error handling process in this function:

The "require" statement is used to check if the sender (the person executing the transaction) is the owner of the contract or not. If the sender is verified it will proceed with the execution, otherwise  the execution is immediately stopped, and an exception is thrown with the error message " You can't open this file". 

To provide an additional layer of validation, an "assert" statement is placed after the require statement. It ensures that the distance given by the user must be more than 0. If the assertion fails, indicating a logical error, the execution is halted, catching any unexpected behavior that may violate the speed logic.

Next, an "if" statement is used to check if the distance / time is less than 0. If the condition is met, the "revert" statement is triggered, causing the transaction to be reverted with the error message "Speed of a body can never be negative". This handles the case whether the speed can be calculated or not.

### More about require, assert and revert
require: The require statement is used to validate certain conditions before proceeding with the execution of a function. It takes a condition as the first argument and an optional error message as the second argument. If the condition evaluates to false, the execution of the function is immediately halted, and any changes made to the state are reverted. An error message can be provided to indicate the reason for the failure. The require statement is typically used for input validation and to ensure certain conditions are met before executing further code.

assert: The assert statement is used to check for conditions that should never evaluate to false. It is typically used to validate internal consistency or invariants of the contract. If the condition provided to assert evaluates to false, it signifies a critical error in the code, and the execution is halted. Unlike require, assert does not allow for recovery or error messages. The purpose of assert is to catch logical errors during development and testing.

revert: The revert statement is used to flag an error and revert the current transaction. It is often used when an unexpected or invalid state is encountered, and there is no safe way to proceed with the execution. The revert statement can optionally include an error message to provide more information about the error. When revert is triggered, all changes made to the state within the transaction are undone, and any Ether sent along with the transaction is returned. It is essential for preventing erroneous states and preserving the integrity of the contract.

In summary, require is used for input validation and conditional checks, assert is used for internal consistency and catching critical errors, and revert is used to flag and revert transactions when encountering unexpected or invalid states. Each statement serves a specific purpose in handling different types of errors and ensuring the integrity of the contract.
# Prequisite
Make sure you have the following software installed on your machine:

1.Solidity compiler version 0.8.7 or compatible

2.Ethereum development environment (e.g., Remix, Truffle, Hardhat, etc.)
# Deployment 
1.Set up your Ethereum development environment.

2.Compile the Solidity code using a compatible compiler.

3.Configure the deployment settings, including gas limit and network parameters.

4.Select the desired network for deployment (e.g., local development network, test network, mainnet).

5.Deploy the contract to the chosen network using your preferred deployment method.

6.Once deployed, interact with the contract by calling its functions and test its functionality.
# License
The code is released under the MIT License, which permits you to use, modify, and distribute it according to the terms of the license.
# Authors
Jaya Singh (https://www.linkedin.com/in/jaya-singh-23b113230).
# Video Walkthrough
https://www.loom.com/share/cc62af5905b24e4f97ef20c1aaa4f765?sid=0df0f1d4-7f59-43fa-a18b-013ce50de81a

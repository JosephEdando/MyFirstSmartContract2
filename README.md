AdvancedStorage

Overview

AdvancedStorage is an advanced smart contract built on top of the SimpleStorage contract. It introduces timestamp functionality, allowing users to store a number and record the exact time of the update.

Features

Inheritance: Extends the functionality of the SimpleStorage contract.

Timestamp Storage: Automatically records the timestamp whenever a number is stored.

Enhanced Data Retrieval: Provides a function to retrieve the stored number along with its timestamp.

Technologies Used

Solidity: Programming language for writing smart contracts.

Remix IDE: Browser-based Integrated Development Environment for Solidity.

Ethereum Blockchain: Deployment and interaction environment

Installation and Setup

Clone or Create the Base Contract:

Ensure the SimpleStorage contract is available in the same directory.

Access Remix IDE:

Go to Remix.

Create the File:

Create a new file named AdvancedStorage.sol.

Copy and Paste the Code:

Paste the above Solidity code into the file.

Compile the Contract:

In Remix, navigate to the "Solidity Compiler" tab and compile the contract.
Deploy the Contract:

Switch to the "Deploy & Run Transactions" tab, and deploy the contract.

Usage

storeNumber:

Stores a new number and automatically updates the timestamp of when the number was saved.

getWithTimestamp:

Retrieves the stored number along with its corresponding timestamp.

License

This project is licensed under the MIT License.

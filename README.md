The AdvancedStorage contract builds upon the foundational functionality of the SimpleStorage contract. It introduces timestamping capabilities, making it possible to track when a favorite number is updated. This project showcases how to utilize inheritance in Solidity to extend and enhance the functionality of a base contract.

Challenges and Resolutions

Challenge 1: Importing and Extending the Base Contract

One of the initial challenges was ensuring that the SimpleStorage contract was properly imported and extended in the AdvancedStorage contract.

Resolution:

Placed the SimpleStorage.sol file in the same directory as AdvancedStorage.sol.
Used Solidity's import statement to include the base contract.
Applied the is keyword to establish inheritance and ensure that the derived contract had access to the base contract’s properties and methods.

Challenge 2:Overriding Functions

Overriding the storeNumber function from the base contract required adherence to Solidity's rules for function overriding, such as matching function signatures and using the override keyword.

Resolution:

Carefully matched the function signature of storeNumber from the SimpleStorage contract.

Used the override keyword to ensure compatibility with the parent contract's function.

Challenge 3: Tracking and Storing Timestamps

Adding a timestamp required understanding the block.timestamp global variable and ensuring it worked seamlessly with the storage logic.

Resolution:

Introduced a timestamp state variable to store the update time.

Updated the overridden storeNumber function to save the block.timestamp whenever a new number was stored.

Challenge 4: Retrieving Multiple Values

Providing users with the ability to retrieve both the stored number and the timestamp simultaneously posed a minor challenge in designing the return structure.

Resolution:

Created the getWithTimestamp function to return a tuple containing both the number and the timestamp.

Used Solidity’s ability to return multiple values from a function.

Lessons Learned

Inheritance and Function Overriding:

Learned how to use inheritance in Solidity to extend and customize contract functionality.
Working with Global Variables:

Gained experience in utilizing block.timestamp to add dynamic behavior to the contract.

Error Resolution in Function Overriding:

Improved understanding of function overriding rules in Solidity, such as the need for the override keyword.

Conclusion

The AdvancedStorage contract demonstrates the effective use of inheritance to extend base functionality and introduces practical features like timestamping. This project helped solidify concepts like inheritance, function overriding, and working with Solidity’s global variables.

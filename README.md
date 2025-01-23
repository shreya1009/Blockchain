# Blockchain


This project is a basic implementation of a blockchain written in Python. It demonstrates the core principles of blockchain, including blocks, cryptographic hashing, and chain validation.


# Features
Creation of a Genesis Block (first block in the chain).
Addition of new blocks with transactions.
Validation of the blockchain to ensure data integrity.
Displaying all blocks in the chain with their details.
Optional Proof of Work for mining blocks (difficulty level configurable).

# Requirements
Ensure you have the following installed:

Python 3.7+


# Execution Instructions
Adding Blocks:

Add new transactions to the blockchain by modifying the blockchain.add_block() calls in the __main__ section.
Displaying the Blockchain:

The display_chain() method outputs the index, timestamp, transactions, hashes, and the previous hash of each block.
Validating the Blockchain:

The validate_chain() method checks the blockchain's integrity:
Ensures each block’s hash is correct.
Validates the link between blocks using previous_hash.
Proof of Work (Optional):

You can use the proof_of_work function to mine a block by finding a hash that meets the difficulty criteria.

# Code Overview
Block Class:

Represents a block in the blockchain.
Includes the following attributes:
index: Position of the block in the chain.
timestamp: Creation time of the block.
transactions: List of transactions stored in the block.
previous_hash: Hash of the preceding block.
hash: The current block's hash, computed using SHA-256.
Includes the calculate_hash() method to compute the block’s hash.
Blockchain Class:

Manages the chain of blocks.
Includes methods to:
create_genesis_block(): Creates the first block.
add_block(transactions): Adds a block with specified transactions.
validate_chain(): Validates the integrity of the entire blockchain.
display_chain(): Prints details of all blocks in the chain.
Proof of Work:

Simulates mining by recalculating the block's hash until it meets the specified difficulty (leading zeros).



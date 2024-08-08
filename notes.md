## Abstract contracts

- Abstract contrcts can have undefined function and defined functions. 
- The undefined functions must the implement by the contracts that inherits it.
- Interfaces can only have undefined functions

- Add to Solidity 101:
Events 
Enums

# CEI
Checks, Effects, Interactions Pattern sometimes call "FREI-PI" (Function Requirements, Effects-Interactions, Prototcol Invariants)

This is an important pattern for coding solidity smart contract function. The goal is that you want to set your functions up where you will do a 

1. Checks
2. Effects (Internal Contact State Changes)
3. Interactions (External Contract Interactions)

# Command to add private key account
cast wallet import myaccount --interactive

# Command to run script
forge script script/Interactions.s.sol:FundSubscription --rpc-url $SEPOLIA_RPC_URL --account myaccount --broadcast

# Types of test
- unit -  Basic tests
- integration - contract interactions
- fork - sudo staging test
- staging - run test on mainnet or testnet

# Verifying contract with foundry
forge verify-contract CONTRACT_ADDRESS  src/Raffle.sol:Raffle --etherscan-api-key $ETHERSCAN_API_KEY --rpc-url $SEPOLIA_RPC_URL --show-standard-json-input > json.json
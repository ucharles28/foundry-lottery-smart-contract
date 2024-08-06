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


cast 
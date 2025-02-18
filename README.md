# Program Registry - IDL Smart Contract

## Overview  
**ProgramRegistry** is a Solidity smart contract designed to register and manage programs along with their associated Interface Definition Language (IDL) URLs. It enables developers to store, update, and retrieve program metadata securely on the Ethereum blockchain.

## Features  
- **Register Programs**: Developers can register programs with a unique name and IDL URL.  
- **Update Program Details**: Only the program owner can update the IDL URL and increment the version.  
- **Retrieve Program Information**: Anyone can query a registered program using its unique program ID.  

## Smart Contract Code  
The contract is implemented in Solidity (`^0.8.19`) and includes the following core functionalities:

- **Program Structure**: Each program has a `name`, `idlUrl`, `version`, and `owner`.  
- **Mapping**: Stores programs using a `bytes32` ID derived from the program name and owner.  
- **Modifiers**: Restricts updates to only the program owner.  
- **Events**: Emits logs when a program is registered or updated.  



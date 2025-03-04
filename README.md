# Blockchain Project

A full-stack blockchain application featuring a React frontend and Hardhat smart contract backend. This project demonstrates the integration of blockchain technology with a modern web interface.

## Project Structure

- `blockchain-app/` - React frontend application
- `contracts/` - Smart contract source files
- `test/` - Smart contract test files
- `ignition/` - Hardhat Ignition deployment modules

## Prerequisites

- React.js (v14 or later)
- npm or yarn
- MetaMask browser extension

## Setup Instructions

1. Clone the repository

```bash
git clone <repository-url>
cd blockchain
```

2. Install backend dependencies

```bash
npm install
```

3. Install frontend dependencies

```bash
cd blockchain-app
npm install
```

## Smart Contract Development

The project uses Hardhat for smart contract development and testing.

### Available Commands

```bash
# Compile contracts
npx hardhat compile

# Run tests
npx hardhat test

# Start local blockchain node
npx hardhat node

# Deploy contracts using Hardhat Ignition
npx hardhat ignition deploy ./ignition/modules/Lock.js
```

## Frontend Application

The frontend is built with React and provides a user interface for interacting with the blockchain.

### Features

- Wallet connection and management
- Smart contract deployment interface
- Blockchain information display
- Token management and transfers
- Deployed contract interaction

### Running the Frontend

From the `blockchain-app` directory:

```bash
npm start
```

The application will be available at https://blockchain.slokesh.com/

## Project Components

### Smart Contracts

- `Lock.sol` - Sample smart contract demonstrating time-locked functionality

### Frontend Components

- `Wallet` - Handles wallet connection and account management
- `DeployContractForm` - Interface for deploying new smart contracts
- `BlockchainInfo` - Displays current blockchain network information
- `DeployedContracts` - Lists and manages deployed contracts
- `TokenActions` - Handles token transfers and management
- `Tokens` - Displays token information and balances

## Testing

### Smart Contract Tests

```bash
npx hardhat test
```

### Frontend Tests

```bash
cd blockchain-app
npm test
```

## Deployment

### Smart Contracts

Deploy smart contracts to the desired network using Hardhat Ignition:

```bash
npx hardhat ignition deploy ./ignition/modules/Lock.js --network <network-name>
```

### Frontend

Build the frontend for production:

```bash
cd blockchain-app
npm run build
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License.

# Hello World Dapp

A simple decentralized application (dapp) built with Truffle, Ganache, and React that demonstrates basic interaction with the Ethereum blockchain. The dapp allows users to set and retrieve a name stored in a smart contract.

## Prerequisites

- [Node.js](https://nodejs.org/) (v14 or higher)
- [Ganache](https://trufflesuite.com/ganache/) - Local blockchain for development
- [MetaMask](https://metamask.io/) - Browser extension for interacting with Ethereum
- [Truffle](https://trufflesuite.com/truffle/) - Development framework for Ethereum

## Installation

1. Clone the repository:
- git clone https://github.com/Chael250/Dapp-hello.git

2. Install dependencies:
- bash
- npm install
- cd client
- npm install


3. Start Ganache and make sure it's running on port 7545

4. Compile and deploy the smart contracts:
- bash
- cd client
- npm run dev


## Project Structure

hello-world-dapp/
├── contracts/ # Smart contracts
│ └── HelloWorld.sol # Main contract
├── migrations/ # Truffle migration files
├── client/ # Frontend React application
├── test/ # Smart contract tests
└── truffle-config.js # Truffle configuration


## Smart Contract

The HelloWorld contract provides two main functions:
- `setName(string memory newName)`: Sets a name in the contract
- `getName()`: Retrieves the currently stored name

## Configuration

### Network Configuration
The project is configured to connect to a local Ganache instance by default:
- Host: 127.0.0.1
- Port: 7545
- Network ID: * (any)

### MetaMask Setup
1. Install MetaMask browser extension
2. Add a new network with the following details:
   - Network Name: Ganache
   - RPC URL: http://127.0.0.1:7545
   - Chain ID: 1337
   - Currency Symbol: ETH
3. Import a Ganache account using its private key

## Development

1. Make sure Ganache is running

2. Deploy contract changes:
- bash
- truffle migrate --reset

3. Run the frontend:
- bash
- cd client
- npm run dev

## Testing

Run the test suite:
- bash
- truffle test

## License

This project is licensed under the MIT License.

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request
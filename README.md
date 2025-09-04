# Harmonia: Decentralized Music Platform

A multi-chain decentralized music platform built on Polygon and Substrate, enabling artists to register tracks, distribute royalties, and create fan tokens.

## 🏗️ Project Structure

```
Harmonia/
├── polygon/                   # Polygon Layer-2 implementation
│   ├── contracts/             # Smart contracts (EVM)
│   ├── docs/                  # Contract documentation
│   ├── test/                  # Contract tests
│   └── scripts/               # Deployment scripts
├── substrate/                 # Substrate main chain implementation
│   ├── track_registry/        # Track registration pallet
│   ├── metadata_registry/     # Metadata and fingerprinting
│   └── governance/            # On-chain governance
├── shared/                    # Common resources
│   ├── docs/                  # Shared documentation
│   ├── types/                 # TypeScript type definitions
│   └── utils/                 # Common utilities
├── bridge/                    # Cross-chain bridge
│   ├── contracts/             # Bridge contracts
│   ├── relayer/               # Bridge relayer service
│   └── docs/                  # Bridge documentation
└── README.md                  # This file
```

## 🚀 Quick Start

### Prerequisites
- Node.js >= 18.0.0
- npm >= 8.0.0
- Rust (for Substrate development)
- Git

### Installation

```bash
# Clone the repository
git clone https://github.com/harmonia/harmonia.git
cd harmonia

# Install dependencies
npm install
```

### Development

```bash
# Build all components
npm run build

# Run tests
npm run test

# Polygon development
npm run polygon:build
npm run polygon:test
npm run dev:polygon

# Substrate development
npm run substrate:build
npm run substrate:test

# Bridge development
npm run bridge:build
npm run bridge:test
npm run dev:bridge
```

## 🔗 Multi-Chain Architecture

### Polygon Layer-2
- **HARM Token**: ERC20 utility token
- **Fan Token Factory**: Create and manage artist fan tokens
- **Payment Gateway**: Handle HARM and USDC payments
- **Royalty Distribution**: Automated royalty payments
- **Governance**: Voting and proposal system

### Substrate Main Chain
- **Track Registry**: Immutable track registration
- **Metadata Registry**: IPFS integration and audio fingerprinting
- **Governance**: On-chain governance with quadratic voting

### Cross-Chain Bridge
- **Asset Transfer**: Move tokens between chains
- **State Synchronization**: Keep track data consistent
- **Oracle Integration**: External data feeds

## 📚 Documentation

- [Whitepaper](./shared/docs/HARMONIA.md)
- [Architecture Overview](./shared/docs/ARCHITECTURE.md)
- [API Documentation](./shared/docs/API.md)
- [Polygon Contracts](./polygon/docs/)
- [Substrate Pallets](./substrate/)
- [Bridge Documentation](./bridge/docs/)

## 🛠️ Technology Stack

- **Blockchain**: Polygon (Layer-2), Substrate (Main Chain)
- **Smart Contracts**: Solidity, ink!
- **Frontend**: React, TypeScript, Web3.js
- **Storage**: IPFS
- **Testing**: Hardhat, Mocha, Chai
- **Development**: Node.js, Rust, Docker

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m "Add some amazing feature"`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🔗 Links

- [Website](https://harmonia.music)
- [Documentation](https://docs.harmonia.music)
- [Discord](https://discord.gg/harmonia)
- [Twitter](https://twitter.com/harmoniamusic)

---

**Built with ❤️ by the Harmonia Team**

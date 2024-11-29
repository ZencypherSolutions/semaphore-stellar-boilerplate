# <h1 align="center">Semaphore Stellar Boilerplate</h1>

<p align="center">
    <a href="https://github.com/semaphore-protocol" target="_blank">
        <img src="https://img.shields.io/badge/project-Semaphore-blue.svg?style=flat-square">
    </a>
    <a href="https://eslint.org/">
        <img alt="Linter eslint" src="https://img.shields.io/badge/linter-eslint-8080f2?style=flat-square&logo=eslint">
    </a>
    <a href="https://prettier.io/">
        <img alt="Code style prettier" src="https://img.shields.io/badge/code%20style-prettier-f8bc45?style=flat-square&logo=prettier">
    </a>
</p>

> **🚧 Work In Progress: Stellar Integration 🚧**
> 
> This boilerplate is currently transitioning from Ethereum to Stellar. The current version maintains Ethereum compatibility and will be updated to support Stellar once the [Semaphore Stellar SDK](https://github.com/ZencypherSolutions/semaphore-stellar-sdk) is complete.

| This repository is structured into two main components: a [web app](./apps/web-app) and [smart contracts](./apps/contracts). The application enables users to create Semaphore identities, join groups, and send anonymous feedback (currently on Ethereum's Sepolia testnet). |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |

## 🪧 About The Project

### What is Semaphore?
Semaphore is a cutting-edge privacy layer leveraging **zero-knowledge proofs** to enable anonymous participation in group activities such as voting, signaling, and endorsements. Users can verify their membership in groups and perform activities without revealing their identity.

### Why Stellar?
Stellar's rapidly growing ecosystem lacks privacy-preserving solutions that are already standard in many EVM chains. Integrating Semaphore with Stellar will bring **proven zero-knowledge privacy technology** to a new blockchain, empowering developers to build secure, private, and decentralized applications for Stellar's expanding user base.

## 🛠 Installation

1. Clone the repository:
```bash
git clone https://github.com/your-username/semaphore-stellar-boilerplate.git
cd semaphore-stellar-boilerplate
```

2. Install dependencies:
```bash
yarn
```

3. Set up environment:
```bash
cp .env.example .env
```

## 📜 Current Usage (Ethereum)

### Local Development
Start the development server:
```bash
yarn dev
```

### Deploy Contracts (Sepolia)
1. Navigate to contracts directory:
```bash
cd apps/contracts
```

2. Deploy the contract:
```bash
yarn deploy --semaphore <semaphore-address> --network sepolia
```

3. Configure web app:
   - Update `apps/web-app/.env.production` with your contract address
   - Copy artifacts from `apps/contracts/artifacts/contracts` to `apps/web-app/contract-artifacts`

> [!NOTE]
> Find Semaphore contract addresses [here](https://docs.semaphore.pse.dev/deployed-contracts)

### Verify Contracts
```bash
yarn verify <contract-address> <semaphore-address> --network sepolia
```

## 🗂️ Repository Features

- **Modular Architecture**: Easily extendable design for different use cases
- **Development Tools**: Complete testing and deployment setup
- **Documentation**: Comprehensive guides and resources
- **Quality Assurance**: Linting and formatting configurations

## 🌐 Related Repositories
The Semaphore Stellar ecosystem includes:
- [Semaphore Stellar Docs](https://github.com/ZencypherSolutions/semaphore-stellar-docs)
- [Semaphore Stellar Contracts](https://github.com/ZencypherSolutions/semaphore-stellar-contracts)
- [Semaphore Stellar SDK](https://github.com/ZencypherSolutions/semaphore-stellar-sdk)

## 💬 Community

Join our community:
- [Semaphore Stellar Telegram](https://t.me/+-9623JNgGjEyNzI5)
- [Semaphore Community](https://t.me/semaphore_community)

## 🛠 Development

### Code Quality
```bash
# Check formatting
yarn prettier

# Format code
yarn prettier:write
```

## 🤝 Contributing

We welcome contributions! Please review our [Contributing Guidelines](https://github.com/ZencypherSolutions/semaphore-stellar-docs/blob/main/CONTRIBUTING.md) before submitting changes.

## ⭐ Acknowledgments

This project represents a bridge between Semaphore's privacy technology and Stellar's blockchain ecosystem. Special thanks to both the Semaphore and Stellar communities for their ongoing support and innovation.
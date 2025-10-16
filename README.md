# 🌐 Decred NodeOps Templates

<div align="center">
  <img src="assets/decred-dcr-logo.jpg" alt="Decred Logo" width="200" height="200">
  
  <h1>Decred NodeOps Templates</h1>
  <p>Complete Decred infrastructure templates for NodeOps platform</p>
  
  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
  [![NodeOps](https://img.shields.io/badge/NodeOps-Compatible-brightgreen)](https://cloud.nodeops.network/marketplace)
  [![Decred](https://img.shields.io/badge/Decred-Official-blue)](https://decred.org)
  [![Docker](https://img.shields.io/badge/Docker-Ready-blue)](https://hub.docker.com/r/virgilbb)
</div>

## 📖 Overview

This repository contains NodeOps-compatible templates for deploying Decred infrastructure:

- **Simple Decred Node** - Basic dcrd node for network participation
- **Decred Pulse Dashboard** - Full monitoring stack with GUI

## 🚀 Available Templates

### 1. Simple Decred Node
**Basic dcrd node for network participation**

- ✅ **Image**: `virgilbb/dcrd:latest`
- ✅ **Resources**: 2 CPU, 4GB RAM, 120GB storage
- ✅ **Network**: Testnet (faster sync)
- ✅ **Cost**: ~$3-5/month

**Perfect for:**
- Network participation
- Learning Decred
- Lightweight deployment

### 2. Decred Pulse Dashboard
**Complete monitoring stack with modern GUI**

- ✅ **Images**: 4-container stack
  - `virgilbb/decred-pulse-dcrd:latest` - Full node
  - `virgilbb/decred-pulse-dcrwallet:latest` - Wallet
  - `virgilbb/decred-pulse-backend:latest` - API
  - `virgilbb/decred-pulse-frontend:latest` - Dashboard
- ✅ **Resources**: 2.2 CPU, 4.5GB RAM, 18GB storage
- ✅ **Network**: Mainnet
- ✅ **Cost**: ~$5-10/month

**Features:**
- 📊 Real-time node monitoring
- 💰 Wallet management
- 🔍 Built-in block explorer
- 📈 Network statistics
- 🎫 Staking ticket tracking

## 🎯 Quick Start

### Deploy Simple Node
```yaml
# Use template: Simple Decred Node
# Just provide RPC password
# Deploy on NodeOps marketplace
```

### Deploy Full Dashboard
```yaml
# Use template: Decred Pulse Dashboard
# Provide RPC and wallet passwords
# Access dashboard via assigned URL
```

## 📊 Resource Comparison

| Template | CPU | RAM | Storage | Network | Cost/Month |
|----------|-----|-----|---------|---------|------------|
| **Simple Node** | 2.0 | 4GB | 120GB | Testnet | ~$3-5 |
| **Pulse Dashboard** | 2.2 | 4.5GB | 18GB | Mainnet | ~$5-10 |

## 🔧 Configuration

### Environment Variables

**Simple Node:**
- `DCRD_RPC_USER` - RPC username (default: decred)
- `DCRD_RPC_PASS` - RPC password (required)
- `DCRD_NETWORK` - Network type (testnet/mainnet)

**Pulse Dashboard:**
- `DCRD_RPC_PASS` - Node RPC password
- `DCRWALLET_RPC_PASS` - Wallet password
- All other variables have defaults

## 📚 Documentation

- **[Simple Node Guide](docs/simple-node.md)** - Basic deployment
- **[Pulse Dashboard Guide](docs/pulse-dashboard.md)** - Full stack deployment
- **[Troubleshooting](docs/troubleshooting.md)** - Common issues
- **[Akash Deployment](docs/akash-deployment.md)** - Alternative deployment

## 🐳 Docker Images

All images are available on Docker Hub:

```bash
# Simple node
docker pull virgilbb/dcrd:latest

# Pulse dashboard stack
docker pull virgilbb/decred-pulse-dcrd:latest
docker pull virgilbb/decred-pulse-dcrwallet:latest
docker pull virgilbb/decred-pulse-backend:latest
docker pull virgilbb/decred-pulse-frontend:latest
```

## 🌐 Deployment Platforms

### NodeOps (Recommended)
- ✅ One-click deployment
- ✅ Managed infrastructure
- ✅ Automatic updates
- ✅ Built-in monitoring

### Akash Network
- ✅ Decentralized deployment
- ✅ Lower costs
- ✅ Community-driven
- ✅ Full control

## 📈 What You Get

### Simple Node Benefits
- 🌐 Support Decred network
- 🔒 Run your own node
- 📊 Basic monitoring
- 💰 Lower resource usage

### Pulse Dashboard Benefits
- 📊 Beautiful web interface
- 💰 Wallet management
- 🔍 Block explorer
- 📈 Real-time statistics
- 🎫 Staking support
- 🔄 Auto-refresh data

## 🛡️ Security

- ✅ Non-root containers
- ✅ Minimal attack surface
- ✅ Secure RPC authentication
- ✅ No private key storage (watch-only)
- ✅ Regular security updates

## 💡 Use Cases

### For Beginners
- Start with Simple Node
- Learn Decred basics
- Low cost entry point

### For Advanced Users
- Use Pulse Dashboard
- Full monitoring capabilities
- Wallet management
- Network analysis

### For Developers
- API access via backend
- Custom integrations
- Real-time data feeds
- Blockchain exploration

## 🔗 Links

- **Decred Official**: [https://decred.org](https://decred.org)
- **NodeOps Platform**: [https://cloud.nodeops.network/marketplace](https://cloud.nodeops.network/marketplace)
- **Docker Hub**: [https://hub.docker.com/r/virgilbb](https://hub.docker.com/r/virgilbb)
- **Akash Network**: [https://akash.network](https://akash.network)

## 🤝 Support

- **GitHub Issues**: [Report bugs or request features](https://github.com/VirgilBB/decred-nodeops/issues)
- **Telegram**: [https://t.me/Cerebro_Virgil](https://t.me/Cerebro_Virgil)
- **Twitter**: [https://x.com/Cerebro_Agent](https://x.com/Cerebro_Agent)
- **Decred Community**: [https://discord.gg/decred](https://discord.gg/decred)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Decred Team** - For building amazing blockchain technology
- **NodeOps** - For providing the deployment platform
- **Akash Network** - For decentralized infrastructure
- **Community** - For feedback and contributions

---

<div align="center">
  <p><strong>Ready to deploy Decred infrastructure?</strong></p>
  <p>
    <a href="https://cloud.nodeops.network/marketplace">🚀 Deploy on NodeOps</a> |
    <a href="https://akash.network">🌐 Deploy on Akash</a> |
    <a href="https://github.com/VirgilBB/decred-nodeops/issues">🐛 Report Issues</a>
  </p>
</div>
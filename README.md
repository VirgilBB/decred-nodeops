# 🚀 Decred Pulse GUI Dashboard - NodeOps Template

Deploy a complete Decred infrastructure with web dashboard on NodeOps and monitor your node with a beautiful GUI interface!

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![NodeOps](https://img.shields.io/badge/NodeOps-Compatible-brightgreen)](https://cloud.nodeops.network/marketplace)
[![Decred](https://img.shields.io/badge/Decred-Mainnet-blue)](https://decred.org)

## 📖 What is This?

This is a NodeOps template that deploys a **complete Decred infrastructure** with a modern web dashboard. Includes full dcrd node, backend API, and React frontend for monitoring and management.

### ✨ Features

- 🚀 **One-Click Deployment** - Complete Decred infrastructure in minutes
- 💰 **Cost-Efficient** - Optimized resources (~$3.50/month)
- 🔒 **Secure** - Multi-service architecture with proper isolation
- 📊 **Real-Time Dashboard** - Monitor sync progress, blocks, and network stats
- 🎯 **Full Node** - Complete dcrd node with RPC access
- 🔄 **Auto-Recovery** - Automatic restarts on failure
- 📈 **Block Explorer** - Built-in blockchain explorer
- 🎫 **Staking Dashboard** - Monitor ticket pool and voting

## 🚀 Quick Start

### Step 1: Deploy on NodeOps

1. Log in to [NodeOps Marketplace](https://cloud.nodeops.network/marketplace)
2. Search for **"Decred Pulse GUI Dashboard"**
3. Click **"Deploy"**
4. (Optional) Customize RPC credentials
5. Click **"Deploy"**

### Step 2: Wait for Sync

- **Initial Setup**: 5-10 minutes for container startup
- **Blockchain Sync**: 24+ hours for full mainnet sync
- **GUI Access**: Dashboard available immediately via NodeOps port forwarding

### Step 3: Access Your Dashboard

- **NodeOps Dashboard**: Use port forwarding to access the web interface
- **Monitor Progress**: Watch real-time sync progress
- **Explore Blockchain**: Use built-in block explorer
- **Check Staking**: Monitor ticket pool status

## 📊 What You're Running

- **dcrd**: Full Decred node with RPC
- **Backend**: Node.js API server
- **Frontend**: React dashboard
- **Resources**: ~400m CPU, 896MB RAM total
- **Cost**: ~$3.50/month on NodeOps

## 🔧 Configuration Options

| Variable | Default | Description |
|----------|---------|-------------|
| `DCRD_RPC_USER` | `decred` | RPC username |
| `DCRD_RPC_PASS` | `decred123` | RPC password |
| `DCRD_NETWORK` | `mainnet` | Network (mainnet/testnet) |

## 📈 Expected Performance

- **Startup Time**: 5-10 minutes for containers
- **Sync Time**: 24+ hours for full blockchain
- **CPU Usage**: ~200-400m actual
- **Memory Usage**: ~512-896MB RAM
- **Network**: Variable based on sync progress

## ❓ Troubleshooting

### Dashboard Not Loading
- **Check port forwarding**: Ensure NodeOps port forwarding is enabled
- **Wait for sync**: Dashboard needs partial sync to show data
- **Check logs**: View container logs in NodeOps dashboard

### Slow Sync Progress
- **Normal for mainnet**: 24+ hours is expected
- **Check network**: Ensure stable internet connection
- **Monitor resources**: Verify adequate CPU/memory allocation

### RPC Connection Issues
- **Verify credentials**: Check RPC username/password
- **Wait for sync**: RPC needs partial blockchain data
- **Check firewall**: Ensure RPC port is accessible

## 🌐 Useful Links

- **Decred Website**: [decred.org](https://decred.org)
- **NodeOps Marketplace**: [cloud.nodeops.network/marketplace](https://cloud.nodeops.network/marketplace)
- **Tutorial**: See [TUTORIAL.md](TUTORIAL.md) for detailed guide
- **Support**: Contact via [Telegram](https://t.me/Cerebro_Virgil) or [Twitter](https://x.com/Cerebro_Agent)

## 📄 License

This template is provided as-is under the MIT License. See [LICENSE](LICENSE) for details.

## 🙏 Acknowledgments

- **Decred Team** - For building the hybrid PoW/PoS consensus
- **NodeOps** - For providing the deployment platform
- **Decred Community** - For continuous development and support

---

**Ready to run a Decred node?** Deploy now on [NodeOps Marketplace](https://cloud.nodeops.network/marketplace)!

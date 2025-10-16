# 📚 Decred Pulse GUI Dashboard - Complete Tutorial

This tutorial will guide you through deploying a complete Decred infrastructure with web dashboard on NodeOps.

## 🎯 What You'll Build

- **Full Decred Node (dcrd)** - Complete blockchain node
- **Backend API** - Node.js server for data processing
- **Web Dashboard** - React frontend for monitoring
- **Real-time Monitoring** - Sync progress, blocks, network stats

## 📋 Prerequisites

- NodeOps account ([cloud.nodeops.network](https://cloud.nodeops.network))
- Basic understanding of blockchain nodes
- Patience for 24+ hour sync time

## 🚀 Step-by-Step Deployment

### Step 1: Access NodeOps Marketplace

1. Go to [cloud.nodeops.network/marketplace](https://cloud.nodeops.network/marketplace)
2. Log in to your NodeOps account
3. Search for **"Decred Pulse GUI Dashboard"**

### Step 2: Configure Deployment

1. Click **"Deploy"** on the Decred template
2. Review the default configuration:
   - **RPC User**: `decred` (change if desired)
   - **RPC Password**: `decred123` (change if desired)
   - **Network**: `mainnet` (recommended)
3. Click **"Deploy"** to start

### Step 3: Monitor Initial Startup

**First 10 minutes:**
- Containers will start up
- Services will initialize
- Port forwarding will be configured
- Dashboard will be accessible

**What to expect:**
```
✅ dcrd: Starting Decred node...
✅ backend: API server starting...
✅ frontend: React app loading...
✅ All services: Running and healthy
```

### Step 4: Access Your Dashboard

1. **In NodeOps Dashboard:**
   - Find your deployment
   - Click on port forwarding
   - Access the web interface

2. **Dashboard Features:**
   - Real-time sync progress
   - Block explorer
   - Network statistics
   - Staking information

### Step 5: Wait for Blockchain Sync

**Timeline:**
- **0-1 hours**: Initial connection and peer discovery
- **1-12 hours**: Downloading blockchain data
- **12-24 hours**: Full sync completion
- **24+ hours**: Dashboard shows complete data

**What you'll see:**
- Sync percentage increasing
- Block height growing
- Network connections establishing
- Dashboard data populating

## 🔧 Configuration Options

### RPC Credentials
```yaml
DCRD_RPC_USER: 'your-username'
DCRD_RPC_PASS: 'your-password'
```

### Network Selection
```yaml
DCRD_NETWORK: 'mainnet'  # or 'testnet'
```

### Resource Allocation
- **dcrd**: 200m CPU, 512MB RAM
- **backend**: 100m CPU, 256MB RAM  
- **frontend**: 100m CPU, 128MB RAM

## 📊 Monitoring Your Node

### Dashboard Sections

1. **Overview**
   - Sync progress
   - Block height
   - Network status
   - Uptime

2. **Block Explorer**
   - Latest blocks
   - Transaction details
   - Address lookups
   - Search functionality

3. **Staking Dashboard**
   - Ticket pool status
   - Voting opportunities
   - Stake statistics
   - Reward tracking

4. **Network Stats**
   - Peer connections
   - Bandwidth usage
   - Memory consumption
   - CPU utilization

### Logs and Debugging

**Access logs in NodeOps:**
1. Go to your deployment
2. Click on each service (dcrd, backend, frontend)
3. View real-time logs
4. Check for errors or warnings

**Common log messages:**
```
dcrd: "Syncing to block height X"
backend: "Connected to dcrd RPC"
frontend: "Dashboard loaded successfully"
```

## ⚠️ Troubleshooting

### Dashboard Won't Load
1. **Check port forwarding**: Ensure NodeOps has enabled it
2. **Wait for startup**: Allow 5-10 minutes for all services
3. **Check logs**: Look for errors in backend/frontend logs
4. **Verify network**: Ensure stable internet connection

### Slow Sync Progress
1. **This is normal**: Mainnet sync takes 24+ hours
2. **Check resources**: Ensure adequate CPU/memory
3. **Monitor network**: Verify stable connection
4. **Be patient**: Full sync is required for complete functionality

### RPC Connection Issues
1. **Verify credentials**: Check username/password
2. **Wait for partial sync**: RPC needs some blockchain data
3. **Check firewall**: Ensure RPC port is accessible
4. **Review logs**: Look for connection errors

### High Resource Usage
1. **Normal during sync**: High CPU/memory usage expected
2. **Monitor allocation**: Ensure resources are adequate
3. **Check for errors**: Look for memory leaks or crashes
4. **Consider upgrade**: May need more resources for large blockchain

## 🎉 Success Indicators

### Your deployment is working when:
- ✅ All three containers are running
- ✅ Dashboard loads without errors
- ✅ Sync progress is visible
- ✅ Block data is updating
- ✅ Network connections are established

### Full functionality achieved when:
- ✅ Sync reaches 100%
- ✅ Dashboard shows complete data
- ✅ Block explorer works
- ✅ Staking dashboard populated
- ✅ All features accessible

## 🔄 Maintenance

### Regular Tasks
- **Monitor sync progress**: Check dashboard regularly
- **Review logs**: Look for errors or warnings
- **Check resources**: Ensure adequate allocation
- **Update if needed**: Keep containers updated

### Long-term Considerations
- **Backup data**: Consider backing up blockchain data
- **Monitor costs**: Track NodeOps usage and costs
- **Stay updated**: Keep up with Decred network updates
- **Community**: Join Decred community for support

## 🌐 Next Steps

### After Full Sync
1. **Explore the dashboard**: Familiarize yourself with features
2. **Check staking**: Monitor ticket pool and voting
3. **Use RPC**: Access Decred RPC for development
4. **Monitor network**: Track Decred network health

### Advanced Usage
1. **RPC Development**: Use the node for building applications
2. **Staking**: Participate in Decred's hybrid consensus
3. **Research**: Analyze blockchain data and statistics
4. **Community**: Contribute to Decred ecosystem

## 🆘 Support

### Getting Help
- **NodeOps Support**: Use NodeOps dashboard support
- **Decred Community**: Join Decred Discord/Telegram
- **Documentation**: Check Decred documentation
- **GitHub Issues**: Report bugs or request features

### Useful Resources
- **Decred Website**: [decred.org](https://decred.org)
- **Decred Documentation**: [docs.decred.org](https://docs.decred.org)
- **NodeOps Support**: [cloud.nodeops.network](https://cloud.nodeops.network)
- **This Template**: [GitHub Repository](https://github.com/VirgilBB/decred-nodeops)

---

**Congratulations!** You now have a complete Decred infrastructure running on NodeOps with a beautiful web dashboard. Enjoy exploring the Decred ecosystem! 🎉

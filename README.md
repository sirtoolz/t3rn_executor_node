# T3rn_executor_node
Setting up T3RN Executor node on VPS

Welcome to t3rn, a Modular Interoperability Layer designed for fast, secure, and cost-efficient cross-chain swapping. t3rn is uniquely positioned to bridge the gaps in blockchain interoperability, offering superior swapping for users and yield for infra providers by becoming t3rn Executors.

Docs : [t3rn docs](https://docs.t3rn.io/intro) | X : [t3rn](https://x.com/t3rn_io)

---

# VPS Options

💻 Contabo VPS Deals 🚀 Buy with Credit Card/Paypal/Crypto Credit card : 

Get powerful VPS solutions with these direct links:  

| **VPS** | **Direct Link**                      | **Specs**                                                                          |
|---------|--------------------------------------|------------------------------------------------------------------------------------|
| VPS 1   | [Contabo VPS 1](https://www.jdoqocy.com/click-101278318-15692486) | 4 vCPU Cores, 4 GB RAM, 100 GB NVMe or 400 GB SSD     |
| VPS 2   | [Contabo VPS 2](https://www.anrdoezrs.net/click-101278318-13796472) | 6 vCPU Cores, 16 GB RAM, 200 GB NVMe or 400 GB SSD  |
| VPS 3   | [Contabo VPS 3](https://www.dpbolvw.net/click-101278318-13796474) | 8 vCPU Cores, 24 GB RAM, 300 GB NVMe or 1.2 TB SSD    |
| VPS 4   | [Contabo VPS 4](https://www.anrdoezrs.net/click-101278318-13796476) | 12 vCPU Cores, 48 GB RAM, 400 GB NVMe or 1.6 TB SSD |


💡 **Get started with the perfect VPS for your needs!** 🚀


----------------------------------------------------------------------------------------------------------------------------------------
### Getting Started with t3rn:
#### Participate as an Executor:
Join the network as an Executor to process transactions and engage in the ecosystem by bidding on orders and executing transactions.

#### Explore t3rn's Bridge UI:
Explore cross-chain swaps with our intuitive Bridge UI. Now live on testnets, it enables fast, secure, and cost-efficient cross-chain transactions.

Task : https://app.galxe.com/quest/t3rn/GC2NYtzDN6
[Answers : C, A, D, C]

Faucet : https://faucet.brn.t3rn.io/

Bridge : https://bridge.t1rn.io 

----------------------------------------------------------------------------------------------------------------------------------------

# Join Crypto Console Community

Join TG : [Crypto Console Telegram](https://t.me/cryptoconsol) | Follow X : [Crypto Console Twitter](https://www.x.com/cryptoconsol) | Subscribe : [Crypto Console Youtube](https://www.youtube.com/@cryptoconsole)

Crypto VPS : [https://vpsdime.com](https://vpsdime.com/a/4418/linux-vps)

----------------------------------------------------------------------------------------------------------------------------------------

### Update and upgrade system packages
```
sudo apt update
sudo apt upgrade
```
### Install fonts
```
sudo apt-get install figlet
figlet -f /usr/share/figlet/starwars.flf

```
### Download t3rn binaries
```
LATEST_VERSION=$(curl -s https://api.github.com/repos/t3rn/executor-release/releases/latest | grep 'tag_name' | cut -d\" -f4)
EXECUTOR_URL="https://github.com/t3rn/executor-release/releases/download/${LATEST_VERSION}/executor-linux-${LATEST_VERSION}.tar.gz"
curl -L -o executor-linux-${LATEST_VERSION}.tar.gz $EXECUTOR_URL

```
### Extract 
```
tar -xzvf executor-linux-${LATEST_VERSION}.tar.gz
rm -rf executor-linux-${LATEST_VERSION}.tar.gz
cd executor/executor/bin

```

### Open screen 
```
screen -S t3rn
```
### Set your preferred Node Environment.
```
export NODE_ENV=testnet
```
### Set your log settings
```
export LOG_LEVEL=debug
export LOG_PRETTY=false
export EXECUTOR_PROCESS_ORDERS=true
export EXECUTOR_PROCESS_CLAIMS=true
export EXECUTOR_MAX_L3_GAS_PRICE=50
export EXECUTOR_PROCESS_PENDING_ORDERS_FROM_API=false
```
### PRIVATE KEYS
Set the PRIVATE_KEY_LOCAL variable of your Executor, Replace with your privatekey
```
export PRIVATE_KEY_LOCAL=<replace your privatekey>
```
### Set Networks
```
export ENABLED_NETWORKS='arbitrum-sepolia,base-sepolia,optimism-sepolia,l1rn'
```
### Start Node
```
./executor
```
You can minimze the screen with CTRL+A+D

To open your screen again:screen -r t3rn

Take a screenshot of running node and post it on discord to get a role.

Discord : https://discord.gg/tW9Zqacw

Join Crypto Console : [Community](https://t.me/cryptoconsol)

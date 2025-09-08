# Irys_CLi

# Step 1
Install Imp dependencies 
```
sudo apt-get update && sudo apt-get upgrade -y
```
```
sudo apt install curl iptables build-essential git wget lz4 jq make protobuf-compiler cmake gcc nano automake autoconf tmux htop nvme-cli libgbm1 pkg-config libssl-dev libleveldb-dev tar clang bsdmainutils ncdu unzip libleveldb-dev screen ufw -y
```

# Step 2
Install node js and npm
```
curl -fsSL https://deb.nodesource.com/setup_20.x | sudo -E bash - && sudo apt install -y nodejs
```

check version
```
node -v
npm -v
```

# Step 3 
CLI Installation 
```
sudo npm i -g @irys/cli
```

verify
```
irys
```


# Step 4 Fund Wallet 
```
irys fund 10000000000000000 \
-n devnet \
-t ethereum \
-w WITHOUT_0x \
--provider-url https://eth-sepolia.public.blastapi.io
```
Replace RPC_URL with your selected network: [https://sepolia.drpc.org](https://chainlist.org/chain/11155111)


# Step 5 Check Balance 
```
irys balance WALLET_ADDRESS   -t ethereum   -n devnet   --provider-url https://eth-sepolia.public.blastapi.io
```

# Step 6 Upload File 
```
irys upload spy.jpg  \
-n devnet \
-t ethereum \
-w PRV_KEY \
--tags spy.jpg jpg \
--provider-url https://eth-sepolia.public.blastapi.io
```

# DONE

# Octra Wallet Generated

![image](https://github.com/user-attachments/assets/7976cdf8-85b4-4acb-9640-8582e4a80ff9)

**You can run via [Github Codespace](https://github.com/codespaces) or VPS server**

**You can now generate a `testnet wallet` by following this instruction**:

### 1. Open your terminal and run:
```
sudo apt update -y && sudo apt upgrade -y
```

### 2. Install Required Packages:
```
sudo apt install htop ca-certificates zlib1g-dev libncurses5-dev libgdbm-dev libnss3-dev tmux iptables curl nvme-cli git wget make jq libleveldb-dev build-essential pkg-config ncdu tar clang bsdmainutils lsb-release libssl-dev libreadline-dev libffi-dev jq gcc screen file nano btop unzip lz4 -y
```

### 3. Download Wallet Generator:
- Run the following to download and extract the wallet generator:
```
wget https://github.com/octra-labs/wallet-gen/releases/download/v4/wallet-generator-linux-x64.tar.gz
tar -xzf wallet-generator-linux-x64.tar.gz
chmod +x wallet-generator
```

### 4. Open port:
```
ufw allow 8888
```


### 5. Then run the wallet generator:
```
./wallet-generator
```
- Open the` Wallet Generator` Web UI
- In your browser, go to: `http://YOUR_SERVER_IP:8888`
- Using Github Codespace, Navigate to `http://localhost:8888`
- You should now see the `Octra Wallet Generator` page.

![image](https://github.com/user-attachments/assets/61d1d0cb-f7c3-4b6d-aff9-4594a350e9f0)

### 6. Generate Your Wallet
- Click "Generate Wallet" on the web interface.
- Save all the information shown, including:
  - Private Key
  - Public Address
  - Mnemonic Phrase

 ### 7. Open new Terminal and Save Wallet Info from File:
 The generator may also give you a text file (`e.g., octra_wallet_kc4Hzdwp_1751027665.txt`). To view it, run:

Example:
![image](https://github.com/user-attachments/assets/cae1ccb8-b371-4941-b953-ff63473038d5)

- So my file is in `octra_wallet_kc4Hzdwp_1751027665.txt`
- Now go to your terminal and run:
```
cat octra_wallet_kc4Hzdwp_1751027665.txt
```
- Replace `octra_wallet_kc4Hzdwp_1751027665.txt` with your actual filename.

### 8. Get Test Tokens (Faucet):
- Visit the Octra Faucet here: https://faucet.octra.network/
- Paste your wallet address start With: `oct`
- Do not check the box that says “I am a validator”
- Click Submit.

### 9. Confirm on Explorer
  - Check if your wallet received tokens using the Octra explorer. You should see your address marked as "confirmed".
 
### 10. Stop the Wallet Generator
  - When done, press `CTRL + C` in the terminal to stop the generator.
 
  More info's HERE: [Twitter](https://x.com/octra/status/1938309788586414288)

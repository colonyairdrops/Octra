# Generate OCTRA Wallet
- Open [CodeSpace](https://github.com/codespaces)
- Select Blank Template
---
## Clone Repository
```
git clone https://github.com/octra-labs/wallet-gen.git
```
```
cd wallet-gen
```
## Install Bun
```
curl -fsSL https://bun.sh/install | bash
```
```
source ~/.bashrc
```
```
bun install
```
```
bun run build
```
```
bun start
```
- A pop-up will appear use it to open the local host browser
- Generate Wallet & Save Everything
- Get [Faucet](https://faucet.octra.network)

---
# Task 1 - Transfer Tokens
- Create New [Codespace](https://github.com/codespaces)

## Install CLI
```
git clone https://github.com/octra-labs/octra_pre_client.git
```
```
cd octra_pre_client
```
```
pip install -r requirements.txt
```
```
cp wallet.json.example wallet.json
```
```
nano wallet.json
```
* Replace following values:
  * `private-key-here`: Privatekey with `B64` format (already saved earlier)
  * `octxxxxxxxx...`: Octra address starting with `oct...`
* Use CTRL X Y & Enter to Exit

```
./run.sh
```
![image](https://github.com/user-attachments/assets/652ea979-2188-436b-bd64-34a65d0cc061)

- Use the UI to send trx to address
- Address to send: `oct7tBXktyKfnMd4Soo4ZDYqiPJdxs9Ezgeh8KaP3CdeUe8`

# Task 2 - Encrypted Transactions
- Create New [Codespace](https://github.com/codespaces)

## Install CLI
```
git clone https://github.com/octra-labs/octra_pre_client.git
```
```
cd octra_pre_client
```
```
pip install -r requirements.txt
```
```
cp wallet.json.example wallet.json
```
```
nano wallet.json
```
* Replace following values:
  * `private-key-here`: Privatekey with `B64` format (already saved earlier)
  * `octxxxxxxxx...`: Octra address starting with `oct...`
* Use CTRL X Y & Enter to Exit

```
./run.sh
```
![image](https://github.com/user-attachments/assets/20a9cbbd-e58f-4833-801e-67e9b6b0a4dc)
- Use the UI and try different trx
- Address to send: `oct7tBXktyKfnMd4Soo4ZDYqiPJdxs9Ezgeh8KaP3CdeUe8`

# Task 3 - OCS01 Test Contract
- If you are starting new do this before proceeding for Task 3
1. Generate Wallet - [Guide](https://github.com/colonyairdrops/Octra#generate-octra-wallet)
2. Install CLI - [Guide](https://github.com/colonyairdrops/Octra#install-cli)

```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
```
source $HOME/.cargo/env
```
```
git clone https://github.com/octra-labs/ocs01-test.git
```
```
cd ocs01-test
```
```
cargo build --release
```
```
cp EI/exec_interface.json .
```
- Copy the `wallet.json` file from octra_pre_client folder to ocs01-test folder
```
./target/release/ocs01-test
```
* Test all functions


---
- Done !! Feel free to ask queries in telegram channel
- Telegram - https://t.me/colonyairdrops
- Youtube - https://www.youtube.com/@ColonyAirdrops
- Twitter - https://x.com/colony_airdrops

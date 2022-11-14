<p align="center">
  <img height="150" height="auto" src="https://user-images.githubusercontent.com/38981255/185994172-0b4e4ea8-f81a-48db-8020-9be619f485b7.png">
</p>

# ALEO PROVER TESTNET NODE

## 1. Overview
snarkOS is a decentralized operating system for private applications. This forms the backbone of Aleo and allows apps to verify and save status in a publicly verifiable way.

## 2. Minimum Specification
Here are the minimum requirements for running an Aleo node:

CPU: 16-core (preferably 32-core)
RAM: 16GB memory (preferably 32GB)
Storage: 128GB disk space
Network: 50 Mbps upload and download bandwidth

# Automatic Installation

```
wget -O prover.sh https://raw.githubusercontent.com/hexskrt/Aleo-Prover/main/prover.sh && chmod +x prover.sh && ./prover.sh
```

choose option number 1 (default)

it will take a few minutes so be patient

# Save Information Account 

Please remember to save the account private key and view key. The following is an example output:

Attention - Remember to store this account private key and view key.

```
 Attention - Remember to store this account private key and view key.

  Private Key  APrivateKey1xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx  <-- Save Me And Use In The Next Step
     View Key  AViewKey1xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx  <-- Save Me
      Address  aleo1xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx  <-- Save Me
```

# Run Prover

To run the node write command below

```
cd snarkOS
screen -R prover
```

```
./run-prover.sh
```

- `ctrl A D` to save the screen so that it runs on your PC background
- If you want to return to the running screen, use the command `screen -Rd prover`

## Uninstall (Use if you want delete node)

```
rustup self uninstall
rm -rf prover.sh
rm -rf snarkOS
```


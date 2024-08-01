<h1 align=center>0G LABS: Da Retriever Guide</h1>

![0_AxKIus_I-soNSp03](https://github.com/user-attachments/assets/eb3cd7ae-d588-4d3a-8096-60be1838a1c5)


# Validator Node
## Hardware Requirement
|Field|Value|
|:----|:----|
|Memory|8 GB|
|CPU|2 cores|
|Bandwidth|100 MBps for Download / Upload|

## Installation
```bash
sudo apt-get update
sudo apt-get install cmake build-essential protobuf-compiler
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
git clone https://github.com/0glabs/0g-da-retriever.git
```

## Config
|Field|Description|
|:----|:----------|
|log_level|Set log level.|
|grpc_listen_address|Server listening address.|
|eth_rpc_endpoint|JSON RPC node endpoint for the blockchain network.|

## Run
```bash
cargo build --release
```
```bash
./target/release/retriever --config ./run/config.toml
```

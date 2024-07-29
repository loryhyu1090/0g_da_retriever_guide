# 0g_da_retriever_guide

![0G-bg](https://github.com/user-attachments/assets/a8a22fba-fc75-41c3-b8f0-9631f72ebef4)

# Hardware Requirement
```
- RAM: 8 GB
- CPU: 2 cores
- Bandwidth: 100 MBps for Download / Upload
```

# Installation
## Install dependencies
```bash
sudo apt-get update
sudo apt-get install cmake build-essential protobuf-compiler
```

## Install rust
```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

## Download the source code
```
git clone https://github.com/0glabs/0g-da-retriever.git
```

# Configuration
|Field|Description|
|:----|:----------|
|`log_level`|Set log level.|
|`grpc_listen_address`|Server listening address.|
|`eth_rpc_endpoint`|JSON RPC node endpoint for the blockchain network.|

# Run
- Build
  ```bash
  cargo build --release
  ```
- Run
  ```bash
  ./target/release/retriever --config ./run/config.toml
  ```

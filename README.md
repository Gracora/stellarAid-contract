# StellarAid Contract

Rust workspace for StellarAid Soroban smart contracts.

## Workspace Structure

```
contracts/
  donation/     # Donation smart contract
  withdrawal/   # Withdrawal smart contract
  campaign/     # Campaign smart contract
sdk/            # Shared SDK (Horizon client, Soroban RPC, keypair utils, config)
worker/         # Background worker binary
scripts/        # Deployment scripts
docs/           # Documentation
```

## Prerequisites

- Rust toolchain (see `rust-toolchain.toml`)
- wasm32 target: `rustup target add wasm32-unknown-unknown`
- Soroban CLI: `cargo install --locked soroban-cli`

## Quick Start

```bash
cp .env.example .env
make build
make test
```

See [docs/DEPLOY.md](docs/DEPLOY.md) for deployment instructions.

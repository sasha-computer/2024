# 2024

Monorepo for my 2024 projects. ZK proofs, L2 tooling, and developer experience.

## ⭐ create-steel-app

A one-command setup script for building ZK execution proof applications on Ethereum using [Steel](https://github.com/risc0/risc0-ethereum). Detects your `cargo-risczero` version and scaffolds the `erc20-counter` example as a skeleton project. Supports both local proving and Bonsai cloud proving. Built to lower the barrier to entry for ZK development.

**Stack:** Bash · Rust · RISC Zero · Foundry · Solidity

→ [browse code](./create-steel-app)

## ⭐ collatz-zk

A ZK proof that a given number satisfies the [Collatz conjecture](https://en.wikipedia.org/wiki/Collatz_conjecture), verified on-chain via RISC Zero. The guest program runs the full Collatz sequence inside the zkVM using `alloy_primitives::U256` for arbitrary precision, and only commits the input number to the journal if it converges to 1. The on-chain verifier then trustlessly confirms the computation without re-executing it.

**Stack:** Rust · RISC Zero zkVM · Solidity · Foundry · Alloy

→ [browse code](./collatz-zk)

## ⭐ greeter-arb

A workshop project for learning L1 → L2 messaging with the Arbitrum SDK. Deploys greeter contracts on both Ethereum Sepolia and Arbitrum Sepolia, then sends a cross-chain message updating the L2 greeter from L1. Built as a hands-on tutorial with step-by-step instructions.

**Stack:** JavaScript · Hardhat · Arbitrum SDK · Ethers.js

→ [browse code](./greeter-arb)

## ⭐ teztap

A Rust rewrite of `@tacoinfra/getTez`, the Tezos testnet faucet tool. The original was a Node.js PoW challenge runner; this version does the same thing but *fast*, because Rust. One command to get ghostnet XTZ without making your CPU cry. 🚰🦀

**Stack:** Rust

→ [browse code](./teztap)

## ⭐ etherlink-website

Fork of the Etherlink.com landing page. Contributed to the marketing site for Etherlink, a Tezos L2.

**Stack:** Next.js · Vercel

→ [browse code](./etherlink-website)

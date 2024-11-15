# Architecture

This document describes the high-level architecture of Foundry.

### `evm/`

Foundry's EVM tooling. This is built around [`revm`](https://github.com/bluealloy/revm) and has additional
implementation of:
- [cheatcodes](./cheatcodes.md): a set of solidity calls dedicated to testing, which can manipulate the environment in which the execution is run

### `config/`

Contains all of Foundry's settings and methods for retrieving them.

### `cli/`

The core `forge` and `cast` cli implementation. Includes all subcommands.

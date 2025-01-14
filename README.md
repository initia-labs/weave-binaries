# Weave binaries

This repository contains the binaries of Weave CLI project.

Weave is a powerful command-line tool designed for managing Initia deployments and interacting with Initia and Rollup nodes.

To get started, download the latest binary from releases and run `weave init`

## Key Features

- **Bootstrap and Run Initia Node**: Set up an Initia node effortlessly. From configuring the desired network and syncing with an official node to running [Cosmovisor](https://github.com/cosmos/cosmos-sdk/tree/main/tools/cosmovisor) for automatic upgrades, all with a single command.
- **Launch Interwoven Rollup**: Create your own Interwoven Rollup in minutes. Choose your preferred VM, customize the challenge period, select the DA option, and more, all with a single command.
- **Set Up and Run OPinit Bots**: [OPinit bots](https://github.com/initia-labs/opinit-bots) are essential for Initia's Optimistic bridge. Weave simplifies the setup process for you.
- **Set Up and Run Relayer**: Easily run a relayer between Initia L1 and any Rollup without navigating through extensive documentation. Currently, only [Hermes](https://github.com/informalsystems/hermes) is supported.

## Available Commands

Weave currently offers the following main commands and subcommands:

### `weave init`

Initializes the Weave CLI, funding the gas station and setting up the configuration.

### `weave gas-station`

Manages the Gas Station account for Weave with the following subcommands:

- `weave gas-station setup`: Sets Gas Station account on Initia and Celestia for funding Weave transactions.
- `weave gas-station show`: Shows Initia and Celestia Gas Station addresses and balances.

### `weave initia`

Manages Initia full node operations with the following subcommands:

- `weave initia init`: Bootstraps your Initia full node.
- `weave initia start`: Starts the initiad full node application.
- `weave initia stop`: Stops the initiad full node application.
- `weave initia restart`: Restarts the initiad full node application.
- `weave initia log`: Streams the logs of the initiad full node application.

### `weave rollup`

Manages Rollups operations with the following subcommand:

- `weave rollup launch`: Launches a new Interwoven Rollup from scratch.
- `weave rollup start`: Starts the rollup application.
- `weave rollup stop`: Stops the rollup application.
- `weave rollup restart`: Restarts the rollup application.
- `weave rollup log`: Streams the logs of the rollup application.

### `weave opinit`

Manages bot for Initia's optimistic bridge with the following subcommands:

- `weave opinit setup-keys` Sets keys for OPinit bots.
- `weave opinit init` Initializes OPinit bots.
- `weave opinit reset` Resets the OPinit bot's database.
- `weave opinit start`: Starts the OPinit bot process.
- `weave opinit stop`: Stops the running OPinit bot process.
- `weave opinit restart`: Restarts the running OPinit bot process.
- `weave opinit log`: Streams the logs of the running OPinit bot process.

### `weave relayer`

Manages relayer between Initia L1 and Rollups with the following subcommands:

- `weave relayer init`: Initializes and configures the Hermes relayer for IBC.
- `weave relayer start`: Starts the Hermes relayer application.
- `weave relayer stop`: Stops the Hermes relayer application.
- `weave relayer restart`: Restarts the Hermes relayer application.
- `weave relayer log`: Streams the logs of the Hermes relayer application.

### `weave upgrade`

Upgrades Weave to the latest or the desired version.

### `weave analytics`

Configures analytics ex. enable/disable data collection

- `weave analytics disable`: Prevents Weave from collecting analytics data.
- `weave analytics enable`: Allows Weave to collect analytics data.

### `weave version`

Shows the current version of Weave.

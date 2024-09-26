# Weave binaries

This repository contains the binaries of Weave CLI project.

Weave is a powerful command-line tool designed for managing Initia deployments and interacting with Initia and Minitia nodes.

To get started, download the latest binary from releases and run `weave init`

## Available Commands

Weave currently offers the following main commands and subcommands:

### `weave init`

Initializes the Weave CLI, funding the gas station and setting up the configuration.

### `weave initia`

Manages Initia full node operations with the following subcommands:

- `weave initia init`: Bootstraps your Initia full node.
- `weave initia start`: Starts the initiad full node application.
- `weave initia stop`: Stops the initiad full node application.
- `weave initia log`: Streams the logs of the initiad full node application.

### `weave minitia`

Manages Minitia operations with the following subcommand:

- `weave minitia launch`: Launches a new Minitia from scratch.

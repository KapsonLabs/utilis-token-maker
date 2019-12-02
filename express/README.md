# Maker Kit: Express Example

**:warning: Maker Kit is in beta for use on Rinkeby only.**

## Setup

Requires [Node.js](https://nodejs.org) `v8.10.0` or above and NPM or [Yarn](https://yarnpkg.com/lang/en/docs/install/).

Environment variables are loaded from a `.env` file in the root directory. The following must be set:

- `ETHEREUM_ACCOUNT` - The private key of an account to use for staking and trading.
- `ETHEREUM_NODE` - The URL of an Ethereum node to connect to.

There is an example `.env.example` that you can copy to `.env` to start with.

### Ethereum Account

To use an existing Ethereum account, set the `ETHEREUM_ACCOUNT` in your `.env` file. Otherwise it's easy to create an account using MetaMask or the `yarn utils:account` script in the [Maker Kit](https://github.com/airswap/airswap-maker-kit) repository. Paste the generated private key into your `.env` file.

### Ethereum Node

To use an existing Ethereum node, set the `ETHEREUM_NODE` in your `.env` file. Otherwise you can create a free account with INFURA. Navigate to https://infura.io/ to create an account and generate an API key and URL.

## Commands

| Command      | Description          |
| :----------- | :------------------- |
| `yarn`       | Install dependencies |
| `yarn test`  | Run maker tests      |
| `yarn start` | Start the maker      |

## Quick Start

The reference Node.js maker is configured to quote `WETH/DAI` at price `0.1` on port `3000`.

### Test and start your maker

First run the tests to check that they pass.

```bash
$ yarn test
```

All should clear. Now start up the maker to accept start accepting requests.

```bash
$ yarn start
info: Server now listening on 0.0.0.0:808
```

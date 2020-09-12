Zoracles Reference Implementation - Open Oracle (From Compound)

Open Oracle

The Open Oracle is a standard developed by Compound and utilized in Zoracles ZKPs reference implementation. Their SDK allows reporters to sign key-value pairs (e.g. a price feed) that interested users can post to the blockchain. The system has a built-in view system that allows clients to easily share data and build aggregates (e.g. the median price from several sources).

Contracts

First, you will need solc 0.6.6 installed. Additionally for testing, you will need TypeScript installed and will need to build the open-oracle-reporter project by running cd sdk/javascript && yarn.

To fetch dependencies run:

yarn install

To compile everything run:

yarn run compile

To deploy contracts locally, you can run:

Contracts

First, you will need solc 0.6.6 installed. Additionally for testing, you will need TypeScript installed and will need to build the open-oracle-reporter project by running cd sdk/javascript && yarn.

To fetch dependencies run:

yarn install

To compile everything run:

yarn run compile

To deploy contracts locally, you can run:

yarn run deploy --network development OpenOraclePriceData

Note: you will need to be running an Ethereum node locally in order for this to work. E.g., start ganache-cli in another shell.

You can add a view in MyView.sol and run (default is network=development):

yarn run deploy MyView arg1 arg2 ...

To run tests:

yarn run test

To track deployed contracts in a saddle console:

yarn run console

Reporter SDK

This repository contains a set of SDKs for reporters to easily sign "reporter" data in any supported languages. We currently support the following languages:

    JavaScript (in TypeScript)
    Elixir

Poster

The poster is a simple application that reads from a given feed (or set of feeds) and posts...
Contributing

Note: all code contributed to this repository must be licensed under each of 1. MIT, 2. BSD-3, and 3. GPLv3. By contributing code to this repository, you accept that your code is allowed to be released under any or all of these licenses or licenses in substantially similar form to these listed above.

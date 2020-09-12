# Zoracles (Reference Implementation x Open Oracle)

Open Oracle

The Open Oracle is a standard developed by Compound and utilized by Zoracles. Their SDK allows reporters to sign key-value pairs (e.g. a price feed) that interested users can post to the blockchain. The system has a built-in view system that allows clients to easily share data and build aggregates (e.g. the median price from several sources).

Zoracles enhances Open Oracle by providing zero-knowledge proofs for confidential data delivery to smart contracts. Our ZKPs have been built with Zokrates to speed the development process and enable deployment on any Open Oracle implementation.

Contracts

Zoracles will be implemented on the following contracts:

OpenZoraclesPriceData - this is where signed prices will be stored

UniswapAnchoredView - prices are anchored to this time-weighted index to set boundaries on acceptable values and prevents adversarial influence 
These main contracts will allow Open Oracle users to upgrade their price feeds to leverage confidentiality of zero-knowledge proofs.

Note: all code contributed to this repository must be licensed under each of 1. MIT, 2. BSD-3, and 3. GPLv3. By contributing code to this repository, you accept that your code is allowed to be released under any or all of these licenses or licenses in substantially similar form to these listed above.

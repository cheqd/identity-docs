# 🆔 Decentralised Identifiers (DIDs)

> **Learn about DIDs**
> If you want to learn about what [DIDs are, please go over to our learning site here.](https://learn.cheqd.io/overview/introduction-to-decentralised-identity/what-is-a-decentralised-identifier-did)

## Multiple options for creating DIDs

There are multiple supported ways to create DIDs on cheqd mainnet and testnet:

1. Enterprise SDKs
   1. [Veramo SDK for cheqd](#dids-with-veramo-sdk-for-cheqd)
2. [DID Registrar](#dids-with-did-registrar)
3. [cheqd CLI](#dids-with-cheqd-cli) (testing purposes only)

> Learn about [cheqd's DID method in our guide here](https://docs.cheqd.io/node/architecture/adr-list/adr-002-cheqd-did-method)

## DIDs with Veramo SDK for cheqd

This documentation describes how you can use the Veramo SDK for cheqd to create, manage and update Decentralised Identifiers (DIDs).

> ⚠️ **Before you begin...**
>
> Make sure you've correctly [configured the cheqd plugin's agent settings](../../guides/software-development-kits-sdks/veramo-sdk-for-cheqd/setup-cli.md) for Veramo CLI

* [Create a DID](create-a-did.md)
* [Querying a DID](query-did.md)
* [Update an existing DID](update-did.md)
* [Deactivate a DID](deactivate-a-did.md)
* [Create an off-ledger holder DID](create-subject-did.md)
* [Manage identity keys](identity-key-handling.md)
* [DID Operations Troubleshooting](did-operations-troubleshooting.md)

## DIDs with DID Registrar

* [Setup DID Registrar](../did-registrar/did-registrar-setup.md)
* [Create a DID](../did-registrar/create-a-did.md)

## DIDs with cheqd CLI

> Note that the cheqd Cosmos CLI is not suitable for use in production environments and should only be used for testing

* [Setup cheqd CLI](../../advanced-features-and-alternatives/developer-guide.md)
* [Create a DID](../../advanced-features-and-alternatives/cheqd-cosmos-cli-for-identity/create-did.md)
* [Query a DID](../../advanced-features-and-alternatives/cheqd-cosmos-cli-for-identity/query-did-and-did-document.md)
* [Update a DID](../../advanced-features-and-alternatives/cheqd-cosmos-cli-for-identity/update-and-manage-did-document.md)
* [Deactivate a DID](../../advanced-features-and-alternatives/cheqd-cosmos-cli-for-identity/deactivate-a-did.md)

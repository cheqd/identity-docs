# Table of contents

## ℹ Overview

* [Identity Documentation for cheqd](README.md)

## 📖 Tutorials

* [🆔 Decentralised Identifiers (DIDs)](tutorials/did-operations/README.md)
  * [Create a DID](tutorials/did-operations/create-a-did.md)
  * [Querying a DID](tutorials/did-operations/query-did.md)
  * [Update an existing DID](tutorials/did-operations/update-did.md)
  * [Deactivate a DID](tutorials/did-operations/deactivate-a-did.md)
  * [Create an off-ledger holder DID](tutorials/did-operations/create-subject-did.md)
  * [Managing identity keys](tutorials/did-operations/identity-key-handling.md)
  * [DID Operations Troubleshooting](tutorials/did-operations/did-operations-troubleshooting.md)
* [📃 Verifiable Credentials and Presentations](tutorials/verifiable-credentials-and-presentations/README.md)
  * [Issue a Verifiable Credential](tutorials/verifiable-credentials-and-presentations/verifiable-credentials.md)
  * [Verify a Verifiable Credential](tutorials/verifiable-credentials-and-presentations/verify-a-verifiable-credential/README.md)
    * [JWT-VC](tutorials/verifiable-credentials-and-presentations/verify-jwt-vc.md)
  * [Create a Verifiable Presentation](tutorials/verifiable-credentials-and-presentations/verifiable-presentations.md)
  * [Verify a Verifiable Presentation](tutorials/verifiable-credentials-and-presentations/verify-presentation.md)
* [🔗 DID-Linked Resources](tutorials/on-ledger-resources/README.md)
  * [Create a DID-Linked Resource](tutorials/on-ledger-resources/create-a-resource.md)
  * [Create a new Resource version within existing Collection](tutorials/on-ledger-resources/create-a-new-resource-version.md)
  * [Create Status List as a Resource](guides/software-development-kits-sdks/veramo-sdk-for-cheqd/using-on-ledger-resources-to-support-statuslist2021.md)
* [🔄 DID Resolver setup](tutorials/DID-resolution.md)
* [🛅 Demo Wallet for identity setup](tutorials/wallet.md)
* [➡ DID Registrar](tutorials/did-registrar/README.md)
  * [Setup DID Registrar](tutorials/did-registrar/did-registrar-setup.md)
  * [Create a DID](tutorials/did-registrar/create-a-did.md)
  * [Create a DID-Linked Resource](tutorials/did-registrar/create-a-resource.md)

## 📑 Guides

* [📦 Software Development Kits (SDKs)](guides/software-development-kits-sdks/README.md)
  * [🛠 Veramo SDK for cheqd](guides/software-development-kits-sdks/veramo-sdk-for-cheqd/README.md)
    * [👉 Setting up Veramo CLI for cheqd](guides/software-development-kits-sdks/veramo-sdk-for-cheqd/setup-cli.md)
    * [🤨 Troubleshooting Veramo CLI setup](guides/software-development-kits-sdks/veramo-sdk-for-cheqd/troubleshooting-setup.md)
  * [🛠 Hyperledger Aries Framework JavaScript](guides/software-development-kits-sdks/hyperledger-aries-framework-javascript.md)
* [🔗 Understanding DID-Linked Resources](guides/did-linked-resources/README.md)
  * [Context for developing DID-Linked Resources](guides/did-linked-resources/context-for-developing-did-linked-resources.md)
  * [Technical composition of DID-Linked Resources](guides/did-linked-resources/technical-composition-of-did-linked-resources/README.md)
    * [Workflow for creating DID-Linked Resources](guides/did-linked-resources/technical-composition-of-did-linked-resources/creating-a-resource.md)
    * [Referencing DID-Linked Resources in VCs](guides/did-linked-resources/technical-composition-of-did-linked-resources/referencing-did-linked-resources-in-vcs.md)
* [🔒 AnonCreds on cheqd](guides/using-on-ledger-resources-to-support-anoncreds/README.md)
  * [Schema Object](guides/using-on-ledger-resources-to-support-anoncreds/schema-object.md)
  * [CredDef Object](guides/using-on-ledger-resources-to-support-anoncreds/creddef-object.md)
  * [Revocation Registry Definition Object](guides/using-on-ledger-resources-to-support-anoncreds/revocation-registry-definition-object.md)
  * [Status List Entry Object](guides/using-on-ledger-resources-to-support-anoncreds/revocation-registry-entry-object.md)
* [🔍 Understanding cheqd DID Resolver](guides/did-resolver.md)
* [Smart Governance](guides/smart-governance/README.md)
  * [Governance File](guides/smart-governance/governance-file.md)
  * [Trust Registry](guides/smart-governance/trust-registry.md)

## 🏗 Architecture

* [Architecture Decision Record (ADR) Process](architecture/README.md)
* [List of ADRs](architecture/adr-list/README.md)
  * [ADR 001: cheqd DID Method](architecture/adr-list/adr-001-cheqd-did-method.md)
  * [ADR 002: DID-Linked Resources](architecture/adr-list/adr-002-did-linked-resources.md)
  * [ADR 003: DID Resolver](architecture/adr-list/adr-003-did-resolver.md)
  * [ADR 004: DID Registrar](architecture/adr-list/adr-004-did-registrar.md)

## 💫 Advanced features and alternatives

* [🤓 Direct interaction with ledger code](advanced-features-and-alternatives/developer-guide.md)
* [🛰 cheqd Cosmos CLI for identity](advanced-features-and-alternatives/cheqd-cosmos-cli-for-identity/README.md)
  * [Creating a DID with cheqd Cosmos CLI](advanced-features-and-alternatives/cheqd-cosmos-cli-for-identity/create-did.md)
  * [Updating existing DIDs with cheqd Cosmos CLI](advanced-features-and-alternatives/cheqd-cosmos-cli-for-identity/update-and-manage-did-document.md)
  * [Deactivating existing DIDs with cheqd Cosmos CLI](advanced-features-and-alternatives/cheqd-cosmos-cli-for-identity/deactivate-a-did.md)
  * [Querying DIDs with cheqd Cosmos CLI](advanced-features-and-alternatives/cheqd-cosmos-cli-for-identity/query-did-and-did-document.md)
  * [Creating a DID-Linked Resource using cheqd Cosmos CLI](advanced-features-and-alternatives/cheqd-cosmos-cli-for-identity/create-resource.md)
  * [Adding a new Resource version](advanced-features-and-alternatives/cheqd-cosmos-cli-for-identity/add-resource-to-existing-collection.md)
* [⚒ VDR Tools CLI with cheqd](advanced-features-and-alternatives/vdr-tools-with-cheqd.md)

## ⚖️ Legal

* [License](LICENSE.md)
* [Code of Conduct](CODE_OF_CONDUCT.md)
* [Security Policy](SECURITY.md)

## 🆘 Support

* [System Status](https://status.cheqd.net)
* [Slack Channel](http://cheqd.link/join-cheqd-slack)
* [Discord](http://cheqd.link/discord-github)

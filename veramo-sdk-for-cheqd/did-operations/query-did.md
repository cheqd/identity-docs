# Querying a DID using Veramo CLI

Follow these instructions to query a DID, read DIDDoc contents, and resolve DID URLs from the cheqd ledger using Veramo CLI.

## Before you begin

* Make sure you've [done the pre-requisite setup](README.md)

## Resolving `did:cheqd` URLs from ledger

### 1. Invoke Veramo CLI's DID resolver function

Use `veramo did resolve` to resolve did

e.g.:

```bash
veramo did resolve did:cheqd:mainnet:zAXwwqZzhCZA1L77ZBa8fhVNjL9MQCHX
```

### 2. Inspect DID/DIDDoc output

The output should look like the following:

```jsonc
{
  "didResolutionMetadata": {
    "contentType": "application/did+json",
    "retrieved": "2022-07-28T15:05:06Z",
    "did": {
      "didString": "did:cheqd:mainnet:zAXwwqZzhCZA1L77ZBa8fhVNjL9MQCHX",
      "methodSpecificId": "zAXwwqZzhCZA1L77ZBa8fhVNjL9MQCHX",
      "method": "cheqd"
    }
  },
  "didDocument": {
    "id": "did:cheqd:mainnet:zAXwwqZzhCZA1L77ZBa8fhVNjL9MQCHX",
    "verificationMethod": [
      {
        "controller": "did:cheqd:mainnet:zAXwwqZzhCZA1L77ZBa8fhVNjL9MQCHX",
        "id": "did:cheqd:mainnet:zAXwwqZzhCZA1L77ZBa8fhVNjL9MQCHX#key1",
        "publicKeyJwk": {
          "crv": "Ed25519",
          "kty": "OKP",
          "x": "jaa70K9yy4Tw-YEsA2T4F10jsQuFdpVJN9LLhjmOUGw"
        },
        "type": "JsonWebKey2020"
    "authentication": [
      "did:cheqd:mainnet:zAXwwqZzhCZA1L77ZBa8fhVNjL9MQCHX#key1"
        ],    
      }
    ]
  },
    "didDocumentMetadata": {
    "created": "2022-05-13T14:01:20Z",
    "versionId": "B55E82F3022593C2A55D08484D658003B1685177197796FA00B56440671DB842"
  }
}
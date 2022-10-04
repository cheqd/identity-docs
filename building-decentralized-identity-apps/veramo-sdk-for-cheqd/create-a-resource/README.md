# 💎 Create a Resource

Follow these instructions to create a new DID and publish the associated DIDDoc on cheqd ledger.

> ⚠️ **Before you begin...**
>
> Make sure you've correctly [configured the cheqd plugin's agent settings](../../../veramo-sdk-for-cheqd/setup-cli.md) for Veramo CLI

## Instructions

### 1. Create a DID

Follow [this](../../../veramo-sdk-for-cheqd/did-operations/) tutorial to generate keys and create a DID.

### 2. Prepare Resource content

Prepare a file with resource and encode it into `base64`. On Unix systems, you can use the following command:

```bash
$ base64 -w 0 resource.txt
<path-to-the-resource-file>
```

Example:

```bash
$ base64 -w 0 resource.txt
SGVsbG8sIHdvcmxk
```

### 3. Create a UUID for the Resource

[UUIDs are used to identify Resources](../../../resources/creating-a-resource.md). On Unix systems, the `uuidgen` tool can be used to generate a new UUID:

```bash
$ uuidgen
e7b662f8-d3f8-4a83-bd00-2cdcd6cc50ab
```

{% hint style="info" %}
Due to a known bug, please make sure that UUIDs generated and submitted to the ledger are in **lower case**.&#x20;
{% endhint %}

### 4. Prepare/edit command arguments

Before creating a Resource, you will need to prepare the `args.json` file. This file can be saved where ever you choose, but the location must be specified in the create Resource command used in Step 5. (By default, it will be saved under the project root directory.)

#### Example file

```json
{
    "kms": "local",
    "payload": {
        "collectionId": "z4ZUuPbs1xyK7y8d",
        "id": "4a71319b-00b1-4db9-bc05-56dc426f7062",
        "name": "TestResource",
        "resourceType": "TextDocument",
        "data": "SGVsbG8sIHdvcmxk"
    },
    "signInputs": [{
        "verificationMethodId": "did:cheqd:testnet:z4ZUuPbs1xyK7y8d#key-1",
        "keyType": "Ed25519",
        "privateKeyHex": "0f5c124886178037952e87e0cdc55d185732577fca19ae877e64ac9ab24a0cc534e5326e70f1a42d785d93048aee806c359ec75a7b06f39253befd1746708438"
    }]
}
```

#### Parameters

* `kms` (default `local`): Key Management System (KMS) to be used for storage;
* `payload`: Resource definition;
  * `collectionId`: The last fragment of the corresponding DIDDoc;
  * `id`: Use output from the previous step here;
  * `name`: Arbitrary human-readable string used to identify the resource
  * `resourceType`: Resource type, such as `CL-Schema`, `JSONSchema2020`, etc
  * `data`: Use output from the step 2 here;
* `signInputs`: Keys used to sign the corresponding DIDDoc. These must match the ones specified in the DIDDoc, otherwise an error will be thrown;
  * `verificationMethodId`: DIDUrl of the verification method where key is published;
  * `keyType` and `privateKeyHex` should match values that you used to create the DIDDoc.

### 5. Create new DID and publish DIDDoc

```bash
veramo execute -m cheqdCreateResource --argsFile path/to/args.json
```

If you do not specify the `--argsFile` in the previous step, you can also paste a JSON inline argument object by using the `--argsJSON` flag followed by the JSON payload.

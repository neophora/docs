# GetNEP5TransferAmountByContractHashDSTAddressTransactionHashTransferIndexSRCAddressInUint64

as an example:

```
TODO
```


## Input

```json
{
    "additionalProperties": false,
    "properties": {
        "ContractHash": {
            "description": "contract hash in big endian",
            "maxLength": 40,
            "minLength": 40,
            "pattern": "^[0-9a-f]{40}$",
            "type": "string"
        },
        "DSTAddress": {
            "description": "neo address of receiver",
            "type": "string"
        },
        "SRCAddress": {
            "description": "neo address of sender",
            "type": "string"
        },
        "TransactionHash": {
            "description": "transaction hash in big endian",
            "maxLength": 64,
            "minLength": 64,
            "pattern": "^[0-9a-f]{64}$",
            "type": "string"
        },
        "TransferIndex": {
            "default": 0,
            "description": "the index of tranfer event in a transaction",
            "minumum": 0,
            "type": "integer"
        }
    },
    "required": [
        "ContractHash",
        "TransactionHash"
    ],
    "type": "object"
}
```

## Output

```json
{
    "type": "integer"
}
```


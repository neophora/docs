# GetNEP5TransferAmountByTransactionHashLETransferIndexInUint64

as an example:

```
TODO
```


## Input

```json
{
    "additionalProperties": false,
    "properties": {
        "TransactionHashLE": {
            "description": "transaction hash in little endian",
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
        "TransactionHashLE"
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


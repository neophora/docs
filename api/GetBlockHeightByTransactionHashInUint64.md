# GetBlockHeightByTransactionHashInUint64

as an example:

```
TODO
```


## Input

```json
{
    "additionalProperties": false,
    "properties": {
        "TransactionHash": {
            "description": "transaction hash in big endian",
            "maxLength": 64,
            "minLength": 64,
            "pattern": "^[0-9a-f]{64}$",
            "type": "string"
        }
    },
    "required": [
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


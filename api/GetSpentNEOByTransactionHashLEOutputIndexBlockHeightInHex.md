# GetSpentNEOByTransactionHashLEOutputIndexBlockHeightInHex

as an example:

```
TODO
```


## Input

```json
{
    "additionalProperties": false,
    "properties": {
        "BlockHeight": {
            "default": 0,
            "description": "block height",
            "minumum": 0,
            "type": "integer"
        },
        "OutputIndex": {
            "default": 0,
            "description": "output index in a transaction",
            "minumum": 0,
            "type": "integer"
        },
        "TransactionHashLE": {
            "description": "transaction hash in little endian",
            "maxLength": 64,
            "minLength": 64,
            "pattern": "^[0-9a-f]{64}$",
            "type": "string"
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
    "description": "binary data encoded in hex format",
    "pattern": "[0-9a-f]+",
    "type": "string"
}
```


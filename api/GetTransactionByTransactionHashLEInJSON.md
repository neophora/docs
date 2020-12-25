# GetTransactionByTransactionHashLEInJSON

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
    "type": "object"
}
```


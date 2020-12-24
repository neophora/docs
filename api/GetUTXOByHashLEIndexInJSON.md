# GetUTXOByHashLEIndexInJSON

get utxo by hash (little endian) in json

## Input

```json
{
    "type": "object",
    "properties": {
        "Hash": {
            "type": "string",
            "minLength": 64,
            "maxLength": 64,
            "pattern": "[0-9a-f]{64}",
            "description": "transaction hash in little endian"
        },
        "Index": {
            "type": "integer",
            "minimum": 0,
            "default": 0,
            "description": "output index in transaction"
        }
    },
    "required": [
        "Hash"
    ],
    "additionalProperties": false
}
```

## Output

```json
{
    "type": "object",
    "description": "extraced utxo data"
}
```

## Examples

TODO

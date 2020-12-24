# GetUTXOByHashIndexInJSON

get utxo by hash (big endian) in json

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
            "description": "transaction hash in big endian"
        },
        "Index": {
            "type": "number",
            "minimum": 0,
            "description": "index in transaction"
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

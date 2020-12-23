# GetSpentNEOByHashIndexInHex

get spentneo by hash (big endian) in hex

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
    "type": "string",
    "pattern": "[0-9a-f]+",
    "description": "spentneo data encoded in hex format"
}
```

## Examples

TODO

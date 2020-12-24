# GetSpentNEOByHashLEIndexHeightInHex

get spentneo by hash (little endian) index height in hex

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
            "type": "number",
            "minimum": 0,
            "description": "index in transaction"
        },
        "Height": {
            "type": "number",
            "minumum": 0,
            "description": "height"
        },
    },
    "required": [
        "Hash",
        "Height",
        "Index"
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

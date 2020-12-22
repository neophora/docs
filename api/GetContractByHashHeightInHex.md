# GetContractByHashHeightInHex

get contract by hash (big endian) height  in hex

## Input

```json
{
    "type": "object",
    "properties": {
        "Height": {
            "type": "number",
            "minumum": 0,
            "description": "height"
        },
        "Hash": {
            "type": "string",
            "minLength": 40,
            "maxLength": 40,
            "pattern": "[0-9a-f]{40}",
            "description": "script hash in big endian"
        }
    },
    "required": [
        "Height",
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
    "description": "binary contract data encoded in hex format"
}
```

## Examples

TODO

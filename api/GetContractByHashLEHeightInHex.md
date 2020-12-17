# GetContractByHashHeightInHex

get contract by hash (little endian) height in hex

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
            "minLength": 64,
            "maxLength": 64,
            "pattern": "[0-9a-f]{64}",
            "description": "sha256^2 hash in little endian"
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

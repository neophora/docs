# GetStorageByHashHeightInHex

get storage by hash (little endian) height in hex

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
            "description": "contract script hash (little endian) + storage key"
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
    "description": "binary storage data encoded in hex format"
}
```

## Examples

TODO

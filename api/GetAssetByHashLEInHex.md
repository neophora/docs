# GetAssetByHashLEInHex

get asset by hash (little endian) in hex

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
            "description": "asset hash in little endian"
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
    "description": "asset data encoded in hex format"
}
```

## Examples

TODO

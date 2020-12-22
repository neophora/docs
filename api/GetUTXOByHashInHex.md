# GetUTXOByHashInHex

get utxo by hash (big endian) in hex

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
            "description": "utxo hash in big endian"
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
    "description": "output data encoded in hex format"
}
```

## Examples

TODO

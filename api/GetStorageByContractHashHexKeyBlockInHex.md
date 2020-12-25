# GetStorageByContractHashHexKeyBlockInHex

as an example:

```
TODO
```


## Input

```json
{
    "additionalProperties": false,
    "properties": {
        "ContractHash": {
            "description": "contract hash in big endian",
            "maxLength": 40,
            "minLength": 40,
            "pattern": "[0-9a-f]{40}",
            "type": "string"
        },
        "HexKey": {
            "description": "hex encoded key",
            "pattern": "[0-9a-f]*",
            "type": "string"
        }
    },
    "required": [
        "ContractHash"
    ],
    "type": "object"
}
```

## Output

```json
{
    "description": "binary data encoded in hex format",
    "pattern": "[0-9a-f]+",
    "type": "string"
}
```


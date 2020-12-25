# GetStorageByContractHashLEHexKeyBlockHeightInHex

as an example:

```
TODO
```


## Input

```json
{
    "additionalProperties": false,
    "properties": {
        "BlockHeight": {
            "default": 0,
            "description": "block height",
            "minumum": 0,
            "type": "integer"
        },
        "ContractHashLE": {
            "description": "contract hash in little endian",
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
        "ContractHashLE"
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


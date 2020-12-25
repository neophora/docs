# GetStorageByContractHashLEKeyHashBlockInHex

as an example:

```
TODO
```


## Input

```json
{
    "additionalProperties": false,
    "properties": {
        "ContractHashLE": {
            "description": "contract hash in little endian",
            "maxLength": 40,
            "minLength": 40,
            "pattern": "[0-9a-f]{40}",
            "type": "string"
        },
        "KeyHash": {
            "description": "sha256^2 hash of key in big endian",
            "maxLength": 64,
            "minLength": 64,
            "pattern": "[0-9a-f]{64}",
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


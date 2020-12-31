# GetNEP5TotalSupplyByContractHashBlockHeightInUint64

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
        "ContractHash": {
            "description": "contract hash in big endian",
            "maxLength": 40,
            "minLength": 40,
            "pattern": "^[0-9a-f]{40}$",
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
    "type": "integer"
}
```


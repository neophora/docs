# GetNEP5TotalSupplyByContractHashLEInUint64

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
            "pattern": "^[0-9a-f]{40}$",
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
    "type": "integer"
}
```


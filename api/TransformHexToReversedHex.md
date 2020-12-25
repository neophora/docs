# TransformHexToReversedHex

as an example:

```
TODO
```


## Input

```json
{
    "additionalProperties": false,
    "properties": {
        "Hex": {
            "description": "hex data",
            "pattern": "^([0-9a-f]{2})*$",
            "type": "string"
        }
    },
    "required": [],
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


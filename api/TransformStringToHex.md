# TransformStringToHex

as an example:

```
TODO
```


## Input

```json
{
    "additionalProperties": false,
    "properties": {
        "String": {
            "description": "string data",
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


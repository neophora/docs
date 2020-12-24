# GetBlockHashByBlockHeightInHex

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


# GetHeaderByBlockHashLEInJSON

as an example:

```
TODO
```


## Input

```json
{
    "additionalProperties": false,
    "properties": {
        "BlockHashLE": {
            "description": "block hash in little endian",
            "maxLength": 64,
            "minLength": 64,
            "pattern": "^[0-9a-f]{64}$",
            "type": "string"
        }
    },
    "required": [
        "BlockHashLE"
    ],
    "type": "object"
}
```

## Output

```json
{
    "type": "object"
}
```


# GetAssetByAssetHashLEInJSON

as an example:

```
TODO
```


## Input

```json
{
    "additionalProperties": false,
    "properties": {
        "AssetHashLE": {
            "description": "asset hash in little endian",
            "maxLength": 64,
            "minLength": 64,
            "pattern": "[0-9a-f]{64}",
            "type": "string"
        }
    },
    "required": [
        "AssetHashLE"
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


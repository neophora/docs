# GetCoinStateByHashIndexHeightInJSON

get coinstate by hash (big endian) index height in json

## Input

```json
{
    "type": "object",
    "properties": {
        "Hash": {
            "type": "string",
            "minLength": 64,
            "maxLength": 64,
            "pattern": "[0-9a-f]{64}",
            "description": "transaction hash in big endian"
        },
        "Index": {
            "type": "integer",
            "minimum": 0,
            "default": 0,
            "description": "output index in transaction"
        },
        "Height": {
            "type": "integer",
            "minumum": 0,
            "default": 0,
            "description": "height"
        },
    },
    "required": [
        "Hash"
    ],
    "additionalProperties": false
}
```

## Output

```json
{
    "type": "object",
    "description": "extraced coinstate data"
}
```

## Examples

TODO

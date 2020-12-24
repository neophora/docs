# GetHeaderByHeightInHex

get header by height in hex

## Input

```json
{
    "type": "object",
    "properties": {
        "Height": {
            "type": "number",
            "minumum": 0,
            "default": 0,
            "description": "height"
        }
    },
    "required": [],
    "additionalProperties": false
}
```

## Output

```json
{
    "type": "string",
    "pattern": "[0-9a-f]+",
    "description": "binary header data encoded in hex format"
}
```

## Examples

TODO

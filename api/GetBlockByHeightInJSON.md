# GetBlockByHeightInJSON

get block by height in json

## Input

```json
{
    "type": "object",
    "properties": {
        "Height": {
            "type": "number",
            "minumum": 0,
            "description": "height"
        }
    },
    "required": [
        "Height"
    ],
    "additionalProperties": false
}
```

## Output

```json
{
    "type": "object",
    "description": "extraced block data"
}
```

## Examples

TODO

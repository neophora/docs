# GetAccountByAccountHashLEBlockHeightInJSON

as an example:

```
TODO
```


## Input

```json
{
    "additionalProperties": false,
    "properties": {
        "AccountHashLE": {
            "description": "account hash in little endian",
            "maxLength": 40,
            "minLength": 40,
            "pattern": "^[0-9a-f]{40}$",
            "type": "string"
        },
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
    "type": "object"
}
```


# GetAccountByAccountHashInJSON

as an example:

```
TODO
```


## Input

```json
{
    "additionalProperties": false,
    "properties": {
        "AccountHash": {
            "description": "account hash in big endian",
            "maxLength": 40,
            "minLength": 40,
            "pattern": "^[0-9a-f]{40}$",
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
    "type": "object"
}
```


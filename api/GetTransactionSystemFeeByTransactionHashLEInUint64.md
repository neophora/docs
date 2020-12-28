# GetTransactionSystemFeeByTransactionHashLEInUint64

as an example:

```
$ curl https://example.neophora.io -d '{"id":1,"jsonrpc":"2.0","method":"GetTransactionSystemFeeByTransactionHashLEInUint64","params":{"TransactionHashLE": "da5e0d3cfbbc02e9cf863c1d97c56e1dc60114f98c957b308eea0eac76ca7ef8"}}'
{"id":1,"result":0,"error":null}
```


## Input

```json
{
    "additionalProperties": false,
    "properties": {
        "TransactionHashLE": {
            "description": "transaction hash in little endian",
            "maxLength": 64,
            "minLength": 64,
            "pattern": "^[0-9a-f]{64}$",
            "type": "string"
        }
    },
    "required": [
        "TransactionHashLE"
    ],
    "type": "object"
}
```

## Output

```json
{
    "type": "integer"
}
```


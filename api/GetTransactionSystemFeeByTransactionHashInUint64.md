# GetTransactionSystemFeeByTransactionHashInUint64

as an example:

```
$ curl https://example.neophora.io -d '{"id":1,"jsonrpc":"2.0","method":"GetTransactionSystemFeeByTransactionHashInUint64","params":{"TransactionHash": "f87eca76ac0eea8e307b958cf91401c61d6ec5971d3c86cfe902bcfb3c0d5eda"}}'
{"id":1,"result":0,"error":null}
```


## Input

```json
{
    "additionalProperties": false,
    "properties": {
        "TransactionHash": {
            "description": "transaction hash in big endian",
            "maxLength": 64,
            "minLength": 64,
            "pattern": "^[0-9a-f]{64}$",
            "type": "string"
        }
    },
    "required": [
        "TransactionHash"
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


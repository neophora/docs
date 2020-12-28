# GetUTXOByTransactionHashOutputIndexInHex

as an example:

```
$ curl https://example.neophora.io -d '{"id":1,"jsonrpc":"2.0","method":"GetUTXOByTransactionHashOutputIndexInHex","params":{"TransactionHash": "0f2c2397cbdf33794489dffae1f9f38f332e58810922ea7f56b0578b99365296", "OutputIndex": 0}}'
{"id":1,"result":"e72d286979ee6cb1b7e65dfddfb2e384100b8d148e7758de42e4168b71792c6001000000000000007335f929546270b8f811a0f9427b5712457107e7","error":null}
```


## Input

```json
{
    "additionalProperties": false,
    "properties": {
        "OutputIndex": {
            "default": 0,
            "description": "output index in a transaction",
            "minumum": 0,
            "type": "integer"
        },
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
    "description": "binary data encoded in hex format",
    "pattern": "[0-9a-f]+",
    "type": "string"
}
```


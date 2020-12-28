# GetUTXOByTransactionHashLEOutputIndexInHex

as an example:

```
$ curl https://example.neophora.io -d '{"id":1,"jsonrpc":"2.0","method":"GetUTXOByTransactionHashLEOutputIndexInHex","params":{"TransactionHashLE": "965236998b57b0567fea220981582e338ff3f9e1fadf89447933dfcb97232c0f", "OutputIndex": 0}}'
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
    "description": "binary data encoded in hex format",
    "pattern": "[0-9a-f]+",
    "type": "string"
}
```


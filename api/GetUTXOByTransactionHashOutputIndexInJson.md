# GetUTXOByTransactionHashOutputIndexInJSON

as an example:

```
$ curl https://example.neophora.io -d '{"id":1,"jsonrpc":"2.0","method":"GetUTXOByTransactionHashOutputIndexInJSON","params":{"TransactionHash": "0f2c2397cbdf33794489dffae1f9f38f332e58810922ea7f56b0578b99365296", "OutputIndex": 0}}'
{"id":1,"result":{"address":"ASH41gtWftHvhuYhZz1jj7ee7z9vp9D9wk","asset":"0x602c79718b16e442de58778e148d0b1084e3b2dffd5de6b7b16cee7969282de7","value":"0.00000001"},"error":null}
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
    "type": "object"
}
```


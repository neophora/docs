# GetUTXOByTransactionHashLEOutputIndexInJSON

as an example:

```
$ curl https://example.neophora.io -d '{"id":1,"jsonrpc":"2.0","method":"GetUTXOByTransactionHashLEOutputIndexInJSON","params":{"TransactionHashLE": "965236998b57b0567fea220981582e338ff3f9e1fadf89447933dfcb97232c0f", "OutputIndex": 0}}'
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
    "type": "object"
}
```


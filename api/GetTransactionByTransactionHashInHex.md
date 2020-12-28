# GetTransactionByTransactionHashInHex

as an example:

```
$ curl https://example.neophora.io -d '{"id":1,"jsonrpc":"2.0","method":"GetTransactionByTransactionHashInHex","params":{"TransactionHash": "f87eca76ac0eea8e307b958cf91401c61d6ec5971d3c86cfe902bcfb3c0d5eda"}}'
{"id":1,"result":"d1014f0400e1f505145a77a5734f7597705b03e18822b70179819cd1fd141dc9dbba918ff7ae1da826e102bb5de626c9ce2753c1087472616e7366657267c5cc1cb5392019e2cc4e6d6b5ea54c8d4b6d11ac000000000000000004fedf6e656f2d6f6e652d696e766f6b653a7b22636f6e7472616374223a22307861633131366434623864346361353565366236643465636365323139323033396235316363636335222c226d6574686f64223a227472616e73666572222c22706172616d73223a5b5b2266726f6d222c22307832376365633932366536356462623032653132366138316461656637386639316261646263393164225d2c5b22746f222c22307866646431396338313739303162373232383865313033356237303937373534663733613537373561225d2c5b2276616c7565222c2231225d5d7dff076e656f2d6f6e65ff0a32313832303037383339201dc9dbba918ff7ae1da826e102bb5de626c9ce270000014140732704575db455e108600bb93e184540256306e7a7b3e46db16e41a6779c0e8a78aa2c115e6d68bf2f938049a53a2b9b7932e6fa4ab68bca488f1758a68801a62321037f5efaf25ffa8c6067f065364621d479b2e08f142c32322ca290e4f47b962568ac","error":null}
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
    "description": "binary data encoded in hex format",
    "pattern": "[0-9a-f]+",
    "type": "string"
}
```


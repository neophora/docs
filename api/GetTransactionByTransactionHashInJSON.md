# GetTransactionByTransactionHashInJSON

as an example:

```
$ curl https://example.neophora.io -d '{"id":1,"jsonrpc":"2.0","method":"GetTransactionByTransactionHashInJSON","params":{"TransactionHash": "f87eca76ac0eea8e307b958cf91401c61d6ec5971d3c86cfe902bcfb3c0d5eda"}}'
{"id":1,"result":{"Type":"InvocationTransaction","Version":1,"Data":{"Script":"BADh9QUUWnelc091l3BbA+GIIrcBeYGc0f0UHcnbupGP964dqCbhArtd5ibJzidTwQh0cmFuc2ZlcmfFzBy1OSAZ4sxObWtepUyNS20RrA==","Gas":"0","Version":1},"Attributes":[{"usage":"Remark14","data":"6e656f2d6f6e652d696e766f6b653a7b22636f6e7472616374223a22307861633131366434623864346361353565366236643465636365323139323033396235316363636335222c226d6574686f64223a227472616e73666572222c22706172616d73223a5b5b2266726f6d222c22307832376365633932366536356462623032653132366138316461656637386639316261646263393164225d2c5b22746f222c22307866646431396338313739303162373232383865313033356237303937373534663733613537373561225d2c5b2276616c7565222c2231225d5d7d"},{"usage":"Remark15","data":"6e656f2d6f6e65"},{"usage":"Remark15","data":"32313832303037383339"},{"usage":"Script","data":"1dc9dbba918ff7ae1da826e102bb5de626c9ce27"}],"Inputs":[],"Outputs":[],"Scripts":[{"invocation":"40732704575db455e108600bb93e184540256306e7a7b3e46db16e41a6779c0e8a78aa2c115e6d68bf2f938049a53a2b9b7932e6fa4ab68bca488f1758a68801a6","verification":"21037f5efaf25ffa8c6067f065364621d479b2e08f142c32322ca290e4f47b962568ac"}],"Trimmed":false},"error":null}
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
    "type": "object"
}
```


# GetAccountByAddressBlockHeightInHex

as an example:

```
$ curl https://example.neophora.io -d '{"jsonrpc": "2.0","id": 1,"method": "GetAccountByAddressBlockHeightInHex","params":{"Address":"AZCcft1uYtmZXxzHPr5tY7L6M85zG7Dsrv","BlockHeight":2400000} }'
{"id":1,"result":"00bf28093023643bb0858a119f0e065b450b14564c000002e72d286979ee6cb1b7e65dfddfb2e384100b8d148e7758de42e4168b71792c60aaef3a201b0100009b7cffdaa674beae0f930ebe6085af9093e5fe56b34a5c220ccdcf6efc336fc500e02d98f9000000","error":null}
```


## Input

```json
{
    "additionalProperties": false,
    "properties": {
        "Address": {
            "description": "neo address",
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
    "description": "binary data encoded in hex format",
    "pattern": "[0-9a-f]+",
    "type": "string"
}
```


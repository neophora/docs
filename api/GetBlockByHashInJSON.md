# GetBlockByHashInJSON

get block by hash in json

## Input

```json
{
    "type": "object",
    "properties": {
        "Hash": {
            "type": "string",
            "minLength": 64,
            "maxLength": 64,
            "pattern": "[0-9a-f]{64}",
            "description": "sha256^2 hash in big endian"
        }
    },
    "required": [
        "Hash"
    ],
    "additionalProperties": false
}
```

## Output

```json
{
    "type": "object",
    "description": "extraced block data"
}
```

## Examples

```sh
curl https://example.neophora.io -d '{"id":1,"jsonrpc":"2.0","method":"GetBlockByHashInJSON","params":{"Hash":"e66c8bf88a93abf37c8b840860dbed67daf70a9a72ae31f977fc0c68e4be8aed"}}'
{"id":1,"result":{"hash":"0xed8abee4680cfc77f931ae729a0af7da67eddb6008848b7cf3ab938af88b6ce6","version":0,"previousblockhash":"0xd500ce5bce17351e9e5a24833499cf80f2d98882793c13b7bbf221ff32a42ccd","merkleroot":"0x38d33aeedf061a4f8b9dfa03f8df5fafe158c661467275f77de723906b0bd1d5","time":1476647853,"index":26,"nonce":"0c463742943483a3","nextconsensus":"APyEx5f4Zm4oCHwFWiSTaph1fPBxZacYVR","script":{"invocation":"40a59973d2e2e752c5d820dd03954ea3c30a0690da11500c456325faef2bcb878c634bc9b8c59d2b5ccd73c750eb6d312d995c66acc4bbf7b1615282405ae7977e4074dee82353c5fe6c5558d2442468b62d9c71041bf3fddd81376e591c2cc8d0795ba3bb9d7444ae26b3acedef3f358101617618d2bf4bf636dc8925038f7f1f4540a800625441293b589fd590cc36d0e61e5e0ed2425d55976b02965e3242ef628b0c6a0cbe2177551bec1849b024cf5ed18cf00c5354bf36a9fc344c23b27297b240a5670cbeae9bd50f1a304e72d9243c8c90832a7ba01b0edb0ae2d7eba08441e26049bd8d0c1eadd830448a9437f72b42d2faeae0221b4ebb0277ea870ceb063640b89e4c5c9cbfcf1bd1b07f8abca1bfc91afd91a6554d4605e3e17f8946d7c839be93bf33e2237a301ca8331a5896e85cb134b21bc624a05beb12f8e1afff96c3","verification":"552102486fd15702c4490a26703112a5cc1d0923fd697a33406bd5a1c00e0013b09a7021024c7b7fb6c310fccf1ba33b082519d82964ea93868d676662d4a59ad548df0e7d2102aaec38470f6aad0042c6e877cfd8087d2676b0f516fddd362801b9bd3936399e2103b209fd4f53a7170ea4444e0cb0a6bb6a53c2bd016926989cf85f9b0fba17a70c2103b8d9d5771d8f513aa0869b9cc8d50986403b78c6da36890638c3d46a5adce04a2102ca0e27697b9c248f6f16e085fd0061e26f44da85b58ee835c110caa5ec3ba5542102df48f60e8f3e01c48ff40b9b7f1310d7a8b2a193188befe1c2e3df740e89509357ae"},"tx":[{"txid":"0x38d33aeedf061a4f8b9dfa03f8df5fafe158c661467275f77de723906b0bd1d5","size":10,"type":"MinerTransaction","version":0,"attributes":[],"vin":[],"vout":[],"scripts":[],"nonce":2486469539}]},"error":null}
```

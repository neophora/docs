# GetBlockByHeightInJSON

get block by height in json

## Input

```json
{
    "type": "object",
    "properties": {
        "Height": {
            "type": "number",
            "minumum": 0,
            "description": "height"
        }
    },
    "required": [
        "Height"
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
$ curl https://example.neophora.io -d '{"id":1,"jsonrpc":"2.0","method":"GetBlockByHeightInJSON","params":{"Height":5}}'
{"id":1,"result":{"hash":"0xff8fe95efc5d1cc3a22b17503aecaf289cef68f94b79ddad6f613569ca2342d8","version":0,"previousblockhash":"0xbde9267017e354b9b9f7d46ffb99db1d6464812838f509ea9ed0085636d220a6","merkleroot":"0x3e5f2fd838822b105931903b7860e6c9ec2e78b7be6233eac5590a2206d6e734","time":1476647460,"index":5,"nonce":"6bf3de3bf042204d","nextconsensus":"APyEx5f4Zm4oCHwFWiSTaph1fPBxZacYVR","script":{"invocation":"4050021bd2ac3a243016d5a633c82a3d63a0d3960f0fe08892fc890f5541bc56dc5001c0409a911bb3198c4de3c30cc198383ccbef4a08c0f59f23cf8569c7e1544033cffaf1178456bf6af140f854b65180413c4daf0d1ba7d3370b40c30f7900fb3c11a17136939c6dd7e117d9ebc0f022503b744fa2de36475456ce330b77ada14044ec2c44e04e0a618d64f7ecdaf9f45acc369010e4ffd411145b7f7a1cf24845d07a57f8711a95941188565a4258bd5cdfa714bbaa008bbf01e1347c84f4bfcc40115060363d8f2c97ab2d09912382327b4f2c35c5f203a57a4c0681cbabe5ccd1e7f3120ab2f34dcf12e9da180a2561c306325055a66d33b6c4e698108298816b400081cd7905e961bcc63715f605203f3492a9d41fa7fedc158fdba583d45a7a40f947c82bfab7bf5b6eb3b9800cc55a82cc54b753c32383bcb282512e0ec598e0","verification":"552102486fd15702c4490a26703112a5cc1d0923fd697a33406bd5a1c00e0013b09a7021024c7b7fb6c310fccf1ba33b082519d82964ea93868d676662d4a59ad548df0e7d2102aaec38470f6aad0042c6e877cfd8087d2676b0f516fddd362801b9bd3936399e2103b209fd4f53a7170ea4444e0cb0a6bb6a53c2bd016926989cf85f9b0fba17a70c2103b8d9d5771d8f513aa0869b9cc8d50986403b78c6da36890638c3d46a5adce04a2102ca0e27697b9c248f6f16e085fd0061e26f44da85b58ee835c110caa5ec3ba5542102df48f60e8f3e01c48ff40b9b7f1310d7a8b2a193188befe1c2e3df740e89509357ae"},"tx":[{"txid":"0x3e5f2fd838822b105931903b7860e6c9ec2e78b7be6233eac5590a2206d6e734","size":10,"type":"MinerTransaction","version":0,"attributes":[],"vin":[],"vout":[],"scripts":[],"nonce":4030865485}]},"error":null}
```
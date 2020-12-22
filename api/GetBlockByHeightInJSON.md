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
curl https://example.neophora.io -d '{"id":1,"jsonrpc":"2.0","method":"GetBlockByHeightInJSON","params":{"Height": 5004565}}'
{
    "id": 1,
    "result": {
        "hash": "0x9a4da114787c713352bc0540b9fb8f225059948078d9a343019f0637075f5644",
        "version": 0,
        "previousblockhash": "0x909d4dbb896a6844dc67e43313a3005cc14422b2833bfb6fd5b348fb7306d57a",
        "merkleroot": "0x43f5d5ee25c50c06faf1267e33a93444c69c5d1dcd3a1f6378ba234b23274c48",
        "time": 1580430540,
        "index": 5004565,
        "nonce": "8c88d4442be4f9af",
        "nextconsensus": "ANuupE2wgsHYi8VTqSUSoMsyxbJ8P3szu7",
        "script": {
            "invocation": "40d8e624b6ae437fe37266875256e16c23052411d36ee3d694831d6393d3dbb34df32f56df963c16dcb2f1217cfe28da452ad939f804e7beb17260175ea7fef97c40f62937589daef337af1349a901ed646138f35f0e6b86fcd238570dec03a6c0171a9074377d7cd958ab27d0652f8549e25c8e840d158c572874e73e494d33ec02408f62484f484e5b81647e666f870236976707bffa0f22622368a9bdd657d6e991219eb7c065ab53a695fe1487e55771607859deb315cd2994e12aad71faad4f0b4011e8e96284f47608efd2df48e300a297a0c0ecdc3ae28c50e6c554d91808049f31d8c5e2b8cce46d46b78b4c2b30c25803457c53d866367e17f471fbd292b1bc40f2f2707f29c6650b46d424907ac755ac8098856c1067c9f1f48bf8c2513b6b28a2b7ca637844a0e9e215f021d70946cc2d9ea4a77dcc0f218b4b0988bd75964f",
            "verification": "5521024c7b7fb6c310fccf1ba33b082519d82964ea93868d676662d4a59ad548df0e7d21025bdf3f181f53e9696227843950deb72dcd374ded17c057159513c3d0abe20b6421035e819642a8915a2572f972ddbdbe3042ae6437349295edce9bdc3b8884bbf9a32103b209fd4f53a7170ea4444e0cb0a6bb6a53c2bd016926989cf85f9b0fba17a70c2103b8d9d5771d8f513aa0869b9cc8d50986403b78c6da36890638c3d46a5adce04a2102ca0e27697b9c248f6f16e085fd0061e26f44da85b58ee835c110caa5ec3ba5542102df48f60e8f3e01c48ff40b9b7f1310d7a8b2a193188befe1c2e3df740e89509357ae"
        },
        "tx": [
            {
                "txid": "0xec19e4ee8b754c0541eb5bbf9caaaded8263a3bb0bb23831a102c69c5aec021b",
                "size": 10,
                "type": "MinerTransaction",
                "version": 0,
                "attributes": [],
                "vin": [],
                "vout": [],
                "scripts": [],
                "nonce": 736426415
            },
            {
                "txid": "0x30368c83d71e48f7300989095bb8e1fcb8b8955a931da67973b240659e1a8e96",
                "size": 202,
                "type": "ContractTransaction",
                "version": 0,
                "attributes": [],
                "vin": [
                    {
                        "txid": "0xfcfc98a3812c5dc16d9c3793188d729c57b131bf85892387021bf87c47ec9884",
                        "vout": 0
                    }
                ],
                "vout": [
                    {
                        "address": "AR5zQt2P6t1GCH9ZSmEWUjZMy2Z7AfULN4",
                        "asset": "0x602c79718b16e442de58778e148d0b1084e3b2dffd5de6b7b16cee7969282de7",
                        "n": 0,
                        "value": "50"
                    }
                ],
                "scripts": [
                    {
                        "invocation": "4091b279e7d13c2a48125278e96081860967f1d6ac61376f276601dc9f12538445c628d8b48a353a4b82013cdb00f0fc14f3a68657e53b7f9b16427f33b9e94c7d",
                        "verification": "21026ec77f7a8155d325743019e29630f81a242fdeeef6d0ff7d920339e88be93412ac"
                    }
                ]
            }
        ]
    },
    "error": null
}

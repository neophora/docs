# GetHashByHeightInHex

get hash by height in hex

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
    "type": "string",
    "pattern": "[0-9a-f]{64}",
    "description": "block hash in hex format"
}
```

## Examples

```sh
curl https://example.neophora.io -d '{"id":1,"jsonrpc":"2.0","method":"GetHashByHeightInHex","params":{"Height":1}}'
{"id":1,"result":"c96c94033911087c387cc77875869817c7617c000f4e39d7a0eeb0388adb82d7","error":null}
```

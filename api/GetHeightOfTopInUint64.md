# GetHeightOfTopInUint64

get height of top in uint64

## Input

```json
{
    "type": "object",
    "properties": {}
}
```

## Output

```json
{
    "type": "number",
    "description": "latest height of blockchain"
}
```

## Examples

```sh
 curl https://example.neophora.io -d '{"id":1,"jsonrpc":"2.0","method":"GetHeightOfTopInUint64","params":{}}'
 {"id":1,"result":583121,"error":null}
```

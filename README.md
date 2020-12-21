# Neophora API Documents

TODO

# Request and Response

Neophora APIs are developed on JSON-RPC over HTTP(s).

request body can we filled as follows:

```json
{
    "jsonrpc": "2.0",
    "id": 1,
    "method": "ping",
    "params": {}
}
```

response body is like:

```json
{
    "id": 1,
    "result": "pong",
    "error": null
}
```

as an example:

```sh
$ curl https://example.neophora.io -X POST -d '{"jsonrpc": "2.0","id": 1,"method": "ping","params": {}}'
{"id": 1,"result": "pong","error": null}
```

# Endpoints

- mainnet <https://mainnet.neophora.io:4443>

# API List

See [API](api)

`Input` describes the `params` in JSON-RPC request while `Output` describes the `result` in JSON-RPC response.

`Input`s and `Output`s are described in [JSON Schema](https://json-schema.org/)

TODO
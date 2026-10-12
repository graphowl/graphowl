# GraphOWL API

[`openapi.json`](openapi.json) is the OpenAPI 3 description of the GraphOWL HTTP API: every route a client can call, with request and response shapes.

- **Errors** are RFC 9457 problem documents.
- **Lists** are keyset-paginated.
- **Authentication** is a bearer token (an OIDC access token).
- **Status:** early access. The surface may change before 1.0; changes are listed in the [changelog](../CHANGELOG.md).

View it in any OpenAPI tool, for example by pasting the raw file URL into <https://editor.swagger.io>, or generate a client with `openapi-generator`.

The file is generated from the product's own contract and cleaned of internal notes; administrative routes are left out. It describes the API only: it does not include the server's source code.

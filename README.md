<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/logo-lockup-dark.svg">
    <img src="assets/logo-lockup.svg" alt="GraphOWL" width="360">
  </picture>
</p>

# GraphOWL

A knowledge graph engine. GraphOWL stores, queries, reasons over and validates connected knowledge — facts from your databases, documents and systems, the vocabulary that gives them meaning, and the rules they must obey. History, reasoning and validation are part of the engine, not add-ons.

It is not a metadata catalog with a graph bolted on. A data catalog is one thing you can build on it; the same engine models a business domain, checks data against an ontology, answers questions across sources and serves context to people and AI agents.

**Status: early access.** The product is under active development and is not yet generally available.

- Website: <https://graphowl.app>
- Live demo: <https://demo.graphowl.app> — password-protected, synthetic data only. To get a login, email <connect@graphowl.app>.

## What this repository is

This is the **public home** of GraphOWL: where releases are announced, where problems are reported and where questions are answered. **It does not contain the product's source code, which is proprietary.**

| What | Where | State |
|---|---|---|
| Release notes | [`CHANGELOG.md`](CHANGELOG.md) | Live |
| Bug reports and feature requests | [Issues](../../issues) | Live |
| Questions and discussion | [Discussions](../../discussions) | Live |
| How to report a vulnerability | [`SECURITY.md`](SECURITY.md) | Live |
| Standards conformance (what is and is not implemented) | [`docs/standards.md`](docs/standards.md) | Live |
| Further documentation | this repository | Planned |
| API specification (OpenAPI) | [`api/openapi.json`](api/openapi.json) | Live |
| Client libraries (Python, TypeScript) | separate repositories, Apache-2.0 | Planned |
| Runnable examples and synthetic sample data | a separate repository, Apache-2.0 | Planned |

"Planned" means exactly that: not published yet, and no date is promised.

## What GraphOWL is

Three layers, one product:

- **Engine** — a triple store with time travel, constraint validation, reasoning and graph query. Every fact keeps its history: nothing is deleted, only retracted.
- **Domain models** — ontologies, glossaries, rules and expectations, kept in the graph itself and reviewed before they take effect. Packs bundle them per domain, so the same engine serves a data catalog, a compliance model or a product domain. Catalog entities, ownership and lineage are one such model, queried like any other fact.
- **Context layer** — ways for people and agents to use the graph: an MCP server, semantic search and APIs.

## Licence

The text in this repository is licensed under [Creative Commons Attribution 4.0](LICENSE). **The GraphOWL name and logos (in `assets/` and `brand/`) are not covered by that licence** — see [`brand/README.md`](brand/README.md). The GraphOWL product itself is proprietary and all rights are reserved. Libraries and examples published in other repositories carry their own licence, stated in each.

## Contact

<connect@graphowl.app>

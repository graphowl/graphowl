# Roadmap

What is built, what is being worked on, and what is not planned. **No dates are promised.** This page is edited when something ships or a decision changes, and the [changelog](CHANGELOG.md) records what shipped.

Status key: ✅ built · 🔧 in progress · 🗒️ planned · ⛔ not planned

## Engine

| Capability | Status |
|---|---|
| Triple store with history and `asOf` queries | ✅ |
| SPARQL 1.1 query | ✅ |
| openCypher subset (labels, properties, relationships, filters, counts) | ✅ subset; some functions not yet supported |
| OWL 2 RL reasoning, derived facts marked | ✅ |
| SHACL-style constraints and quality expectations | ✅ with [stated gaps](docs/standards.md) |
| Virtual graphs (query a source in place) | ✅ |
| Keyword and semantic search | ✅ (semantic needs an embedding model) |
| SHACL rules, reusable SPARQL constraint components | 🗒️ |
| RDF 1.2 triple terms (`rdf:reifies`) | 🗒️ |
| RDF/XML and TriG over the API | 🗒️ |
| Federated query (SPARQL 1.2) | ⛔ not claimed |

## Semantic access and governance

| Capability | Status |
|---|---|
| Virtual graphs: query a source in place through an approved mapping | ✅ |
| Source-to-model mappings with review, workspace isolation | ✅ |
| Competency questions run against a model and a sample (coverage) | ✅ |
| Model diffs and model health reports | ✅ |
| Ontology-aware planning across several sources (pushdown, transfer cost) | 🗒️ |
| Change-impact analysis before a model or mapping change is approved | 🗒️ |
| Answer-level traces: question, mapping, generated source query, source rows | 🗒️ |
| Business questions as regression tests on every proposed change; pack quality scorecard | 🗒️ |
| Governed writes through virtual graphs | 🗒️ |
| Versioning of ontology, mappings, rules and vocabulary together, with rollback | 🗒️ |
| Detecting and repairing mappings when a source schema changes | 🗒️ |
| Semantic guardrails: check an agent's request against permitted classes, relations and policies before it runs | 🗒️ |

## People and agents

| Capability | Status |
|---|---|
| Console: workspaces, model review, graph exploration | ✅ |
| MCP server (101 tools) with grants and recorded refusals | ✅ |
| HTTP API (469 operations) and OpenAPI description | ✅ |
| Client libraries: ingestion (Python, TypeScript), Python client | ✅ early access |
| Publish the libraries to PyPI and npm | 🗒️ |

## Running it

| Capability | Status |
|---|---|
| Hosted demo | ✅ password-protected |
| Early-access container (amd64, arm64) with an evaluation licence | 🔧 image built; registry access being set up |
| Evaluation licence reviewed by counsel | 🔧 |
| Helm chart | 🗒️ |
| Published benchmarks with the method that produced them | 🗒️ |

## Documentation

| Item | Status |
|---|---|
| Quickstart, concepts, guides, cookbooks | ✅ [docs.graphowl.app](https://docs.graphowl.app) |
| API reference and MCP tool reference (generated) | ✅ |
| More cookbooks and a pack-format guide | 🗒️ |

## How to influence it

Open a [feature request](../../issues/new?template=feature_request.yml) or start a [discussion](../../discussions). Say what you are trying to do, not only the feature you imagine: it changes what we build.

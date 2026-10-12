# Getting help

| You want to | Do this |
|---|---|
| Learn how something works | Start at the [documentation](https://docs.graphowl.app): quickstart, concepts, guides, cookbooks |
| Check whether something is supported | [Known limits](https://docs.graphowl.app/reference/limits/) and the dated [standards page](docs/standards.md) |
| Ask a question | [Discussions](../../discussions) |
| Report a bug | [Open an issue](../../issues/new/choose) with the version, the route or tool, the request and what happened |
| Suggest a feature | A [feature request](../../issues/new?template=feature_request.yml), describing the problem you want solved |
| Report a vulnerability | **Not in public.** See [SECURITY.md](SECURITY.md) |
| Ask for a demo login, or access to the early-access container | Email <connect@graphowl.app> |

## What helps us help you

- The **server version** (`GET /health` returns it) and how you run it (demo, container, platform).
- The **exact request** (remove secrets) and the **response**, including the `type` and `detail` of an error.
- What you expected instead.
- For a query that returns nothing: whether the pattern is inside `GRAPH ?g { ... }` (imported facts live in named graphs).

## Response times

GraphOWL is in early access and maintained by a small team. We read everything; we do not promise a response time. Security reports are acknowledged within five working days.

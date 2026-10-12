# Run GraphOWL yourself (early access)

A PostgreSQL database with pgvector and the GraphOWL server, started with Docker Compose. **For evaluation only**, under the [early-access evaluation licence](../legal/EVALUATION-LICENSE.md) (draft). Not for production.

## 1. Request access

Email <connect@graphowl.app> with your name, organisation, your GitHub username and what you want to evaluate. We add you as a reader of the private container package and reply with the image tag.

## 2. Start it

```bash
echo YOUR_TOKEN | docker login ghcr.io -u YOUR_GITHUB_USERNAME --password-stdin   # a token with read:packages
cp .env.example .env        # set POSTGRES_PASSWORD, check GRAPHOWL_IMAGE
docker compose up -d
curl http://localhost:8080/health      # {"status":"alive","version":"0.1.0"}
```

Open <http://localhost:8080> for the console. The server applies its database migrations at startup.

## 3. Try it

Follow the [quickstart](https://graphowl.app/docs/start/quickstart/) against `http://localhost:8080` instead of the demo. Load the [sample dairy database](https://github.com/graphowl/examples/tree/main/dairy-cooperative) to have something to explore.

## Things to know

- **Open mode.** With no identity provider configured, the server accepts every request and says so at startup. The compose file binds it to `127.0.0.1` for that reason. To let others reach it, configure authentication first: [Authentication](https://graphowl.app/docs/operators/authentication/).
- **Architectures.** Images are published for `linux/amd64` and `linux/arm64`.
- **Data.** Everything is in the `pgdata` volume. Back it up with `pg_dump`. The server sends nothing to us.
- **Stop and clean up:** `docker compose down` (keeps data) or `docker compose down -v` (deletes it).

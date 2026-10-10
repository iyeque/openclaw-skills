# Unified Web Search examples

## Search public web sources

```bash
node skills/unified-web-search/index.js \
  --query "latest climate policy" \
  --sources '["tavily"]' \
  --allow-network \
  --max_results 5
```

The query is sent to Tavily only when `--allow-network` is present.

## Search local workspace content

```bash
node skills/unified-web-search/index.js \
  --query "meeting notes" \
  --sources '["local"]' \
  --allow-local \
  --max_results 10
```

Local search is bounded to the documented workspace folders and requires explicit opt-in.

# DataLeads Change Monitor (GitHub Action)

Check a URL for changes since its last snapshot and return the diff report as JSON.

Calls the DataLeads API endpoint `POST /v1/diff` and writes the JSON response to `dataleads-result.json` plus the `result` output.

## Usage

```yaml
steps:
  - uses: DataLeadsPRO/change-monitor-action@v1
    with:
      url: https://example.com
      api_key: ${{ secrets.DATALEADS_API_KEY }}
```

Get a client key at [data.dataleads.pro](https://data.dataleads.pro).

## License

MIT

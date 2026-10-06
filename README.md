# Max Streltcoff

I run reference sites built on sourced, dated data. Each one has a public
read-only [MCP](https://modelcontextprotocol.io) server, so AI agents can query
the same records the pages show.

## MCP servers

- **[ImmigrationDB](https://immigrationdb.com/)** — `https://immigrationdb.com/mcp` · [immigrationdb-mcp](https://github.com/gospodindark-stack/immigrationdb-mcp)
  27,000+ cities, visa and residence routes, passport entry rules, cost of
  living, salaries, safety, air quality and climate; every value has a source
  and a date.
- **[padel.how](https://padel.how/)** — `https://padel.how/mcp` · [padel-how-mcp](https://github.com/gospodindark-stack/padel-how-mcp)
  Reviewed padel rackets: scores, specs, comparisons and dated retailer offers.
- **[Pickleball3](https://pickleball3.com/)** — `https://pickleball3.com/mcp` · [pickleball3-mcp](https://github.com/gospodindark-stack/pickleball3-mcp)
  Reviewed pickleball paddles: scores, measured specs, comparisons and verified
  purchase links.

All three use Streamable HTTP and need no key or account. To connect them in
one go:

```json
{
  "mcpServers": {
    "immigrationdb": { "url": "https://immigrationdb.com/mcp" },
    "padel-how": { "url": "https://padel.how/mcp" },
    "pickleball3": { "url": "https://pickleball3.com/mcp" }
  }
}
```

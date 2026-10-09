# All New Homes plugin for Claude

Find new-construction homes in supported US cities from Claude. Search a city by
price, bedrooms, bathrooms, square footage, builder, and home type, then read
listing details with links to [All New Homes](https://allnew.homes) and the
builder's own page.

The plugin connects Claude to the read-only All New Homes MCP server at
`https://mcp.allnew.homes/mcp` and adds a skill that guides searches. It is free
and needs no All New Homes account.

## Install

In Claude Code:

```sh
claude plugin marketplace add polyfront/allnew-homes-plugin
claude plugin install allnew-homes@polyfront
```

Or run `/plugin marketplace add polyfront/allnew-homes-plugin` inside a session
and install `allnew-homes` from the `polyfront` marketplace.

## Try it

- "Find new-construction homes in Austin, Texas under $500,000 with at least 3 bedrooms."
- "Which builders have new homes in Parrish, Florida?"
- "Tell me more about the first home and give me the builder's link."

## Tools

| Tool | What it does |
| --- | --- |
| `find_markets` | Finds supported cities by a name prefix of at least 3 characters and lists their builders. |
| `search_homes` | Searches one city with price, bed, bath, size, builder, and home-type filters. |
| `get_home` | Reads current facts and source links for one listing. |

All tools are read-only. The plugin cannot access website accounts, save homes,
contact builders, book tours, or submit offers.

## Coverage and limits

Listings come from public builder inventory and refresh daily. A search covers
one city, not its metro area. Results are grouped by builder, then price, so the
first page is not the cheapest homes in the city. Confirm price, incentives,
completion timing, and availability with the builder. All New Homes is an
informational service, not a real-estate broker or agent.

## Privacy and support

- Plugin details: <https://allnew.homes/plugin>
- Privacy policy: <https://allnew.homes/privacy>
- Terms of service: <https://allnew.homes/terms>
- Support: [admin@allnew.homes](mailto:admin@allnew.homes)

## License

[MIT](LICENSE) © PolyFront LLC

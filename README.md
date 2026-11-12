# Alba.design MCP Server

The hosted MCP server of **[Alba.design](https://alba.design)** — the website and online store builder for entrepreneurs and small businesses.

This repository documents the server. The service itself runs remotely at [`https://alba.design/mcp`](https://alba.design/mcp) — nothing to install or run locally.

- **Endpoint:** `https://alba.design/mcp`
- **Transport:** Streamable HTTP
- **Authentication:** none (🔓 public endpoint)

## Tools

| Tool | What it does |
|---|---|
| `createWebsite` | Creates a website or online store draft from a plain-language description and returns a claim-and-edit link. |
| `getFeatures` | Lists the features of all versions or of a specific one, with documentation links. |
| `getPrices` | Pricing of each version (EUR, USD and more currencies). |
| `supportSearch` | Searches the platform documentation and FAQ in the user's language. |

## Quick start

Add the server to any MCP-capable client (Claude Desktop, Cursor, and others):

```json
{
  "mcpServers": {
    "alba": {
      "url": "https://alba.design/mcp"
    }
  }
}
```

Then try: *"Create a website called My Bakery, professional style, with an online store."*

The assistant calls `createWebsite`, and you receive a link to claim and edit your new site. Websites created through the MCP server start on the free version — no credit card required.

## Links

- Homepage: <https://alba.design>
- Pricing: <https://alba.design/price>
- Feature overview: <https://alba.design/list>
- Glama connector: <https://glama.ai/mcp/connectors/design.alba/albadesign>
- llms.txt: <https://alba.design/llms.txt>

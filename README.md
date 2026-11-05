# Bot Shelf MCP connector

Search [Bot Shelf](https://botshelf.dev), an independent directory of 9,000+ community Grok Bots, from any MCP client. Describe a job in plain words and get bots that fit, each with its creator credited and a link that adds it in Grok.

```
https://mcp.botshelf.dev/mcp
```

Remote server over streamable HTTP. No account or API key needed. It's free and read-only, apart from suggesting a bot.

## Tools

| Tool | What it does |
|---|---|
| `find_bots` | Finds bots for a job you describe in plain words, best match first, with a link that adds each one in Grok. |
| `get_bot` | One bot's full listing, from its x.ai/bot share link or its Bot Shelf page. |
| `latest` | The bots most recently added to Bot Shelf. |
| `list_categories` | The categories, with how many bots each has. |
| `suggest_bot` | Suggests a Grok Bot for Bot Shelf. A person reviews every suggestion before it's listed. |

## Add it to Grok Bot

In Grok Bot's settings, add a custom connector named **Bot Shelf** with the address `https://mcp.botshelf.dev/mcp`. Then ask: "Find me a bot on Bot Shelf that chases unpaid invoices."

Full setup steps: [botshelf.dev/connector](https://botshelf.dev/connector/)

## Add it to other MCP clients

```json
{
  "mcpServers": {
    "bot-shelf": {
      "type": "http",
      "url": "https://mcp.botshelf.dev/mcp"
    }
  }
}
```

## Plain files

Prefer files to a connector? See [botshelf.dev/llms.txt](https://botshelf.dev/llms.txt).

## About

Bot Shelf is made by Nomis ([@cradrrat](https://x.com/cradrrat)). Bot listings belong to their creators. It isn't affiliated with xAI or X.

The connector's source code isn't published here. This repository is its public listing page.

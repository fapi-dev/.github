<p align="center">
  <img src="https://raw.githubusercontent.com/fapi-dev/.github/main/profile/assets/banner.png" alt="FAPI" width="320">
</p>

# FAPI

Open-source utilities for the [FAPI](https://fapi.iisis.ru) auto-parts platform — MCP servers, OpenAPI specs, and client libraries for OEM cross-references, vehicle applicability, and parts lookup.

## Try it in 2 minutes

Use [Claude Desktop](https://claude.ai/download), [Cursor](https://cursor.sh), or any MCP client. Install [`fapi-mcp`](https://github.com/fapi-dev/fapi-mcp) and drop this into your MCP config:

```json
{
  "mcpServers": {
    "fapi-catalog": {
      "command": "uvx",
      "args": ["fapi-mcp"],
      "env": { "FAPI_API_KEY": "<paste-demo-key-here>" }
    }
  }
}
```

Get the current public demo key (shared and rotated periodically — fine for evaluation, not for production load):

```bash
curl -s https://gist.githubusercontent.com/serp83/652d191745773ef6d8b5a0a689479cd6/raw/demo-key.txt
```

Then ask your assistant: _"Find cross-references for MANN W 75/3 with at least 2 positive ratings."_

## What's published

| Repo | What it is |
|---|---|
| [`fapi-mcp`](https://github.com/fapi-dev/fapi-mcp) | MCP server for the Catalog API. 7 tools, on [PyPI](https://pypi.org/project/fapi-mcp/). |
| [`catalog-openapi`](https://github.com/fapi-dev/catalog-openapi) | OpenAPI 3.0 spec for the Catalog API. [Live docs](https://fapi-dev.github.io/catalog-openapi/). |

## Products this org integrates with

- **Catalog by Make** — make / model / modification → parts catalog with OEM cross-references.
- **Vindec** — VIN → catalog ID, drop-in for catalog-driven applications.

## Production access

Demo keys are for evaluation. For production use, contact `development.iisis@gmail.com` or visit **[fapi.iisis.ru](https://fapi.iisis.ru)**.

---

<sub>Maintained by the team behind <a href="https://iisis.ru">iisis.ru</a>.</sub>

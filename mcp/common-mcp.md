## Serena

```
 claude mcp add-json "serena" '{"command":"uvx","args":["--from","git+https://github.com/oraios/serena","serena-mcp-server"]}'
```

## Playwright

```sh
claude mcp add playwright npx @playwright/mcp@latest
```

## Context7

<summary><b>Install in Claude Code</b></summary>

Run this command. See [Claude Code MCP docs](https://docs.anthropic.com/en/docs/agents-and-tools/claude-code/tutorials#set-up-model-context-protocol-mcp) for more info.

#### Claude Code Remote Server Connection

```sh
claude mcp add --transport http context7 https://mcp.context7.com/mcp
```

Or using SSE transport:

```sh
claude mcp add --transport sse context7 https://mcp.context7.com/sse
```

#### Claude Code Local Server Connection

```sh
claude mcp add context7 -- npx -y @upstash/context7-mcp
```

</details>

<details>
<summary><b>Install in Claude Desktop</b></summary>

Add this to your Claude Desktop `claude_desktop_config.json` file. See [Claude Desktop MCP docs](https://modelcontextprotocol.io/quickstart/user) for more info.

```json
{
  "mcpServers": {
    "Context7": {
      "command": "npx",
      "args": ["-y", "@upstash/context7-mcp"]
    }
  }
}
```

</details>

# MemoryRelay Skills for Claude Code

Claude Code plugin marketplace for [MemoryRelay](https://memoryrelay.com).

## Installation

```bash
# Add the marketplace
claude plugins add-marketplace memoryrelay/memory-relay-skills

# Install the plugin
claude plugins install memoryrelay@memoryrelay
```

Or manually add to `~/.claude/plugins/known_marketplaces.json`:

```json
{
  "memoryrelay": {
    "source": {
      "source": "github",
      "repo": "memoryrelay/memory-relay-skills"
    }
  }
}
```

Then enable in your project's `.claude/settings.json`:

```json
{
  "enabledPlugins": {
    "memoryrelay@memoryrelay": true
  }
}
```

## Skills

| Skill | When to Use |
|-------|-------------|
| `memory-workflow` | Session lifecycle, storing/retrieving memories, tiers, deduplication |
| `decision-tracking` | Architectural decision records, check before deciding, supersede outdated |
| `pattern-management` | Reusable conventions, search before creating, adopt across projects |
| `project-orchestration` | Load project context, check cross-project impact, manage dependencies |
| `entity-and-context` | Knowledge graphs, link entities to memories, enriched recall |

## Prerequisites

MemoryRelay tools must be available via the [MemoryRelay MCP server](https://github.com/memoryrelay/mcp-server) or the [OpenClaw plugin](https://github.com/memoryrelay/openclaw-plugin).

## License

MIT

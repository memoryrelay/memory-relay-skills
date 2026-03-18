# MemoryRelay Skills

Guided workflow skills for [MemoryRelay](https://memoryrelay.com) — persistent memory, architectural decisions, reusable patterns, project orchestration, and knowledge graphs for AI agents.

## Skills

| Skill | When to Use |
|-------|-------------|
| `memory-workflow` | Starting a session, storing/retrieving memories, managing tiers and deduplication |
| `decision-tracking` | Making architectural choices, checking for existing decisions, superseding outdated ones |
| `pattern-management` | Establishing reusable conventions, searching before creating, adopting across projects |
| `project-orchestration` | Loading project context, checking cross-project impact, managing dependencies |
| `entity-and-context` | Building knowledge graphs, linking entities to memories, enriched recall |

## Installation

### Claude Code

```bash
# Add the marketplace
claude plugins add-marketplace memoryrelay/memory-relay-skills

# Install the plugin
claude plugins install memoryrelay@memoryrelay
```

Or add to your project's `.claude/settings.json`:

```json
{
  "enabledPlugins": {
    "memoryrelay@memoryrelay": true
  }
}
```

### Prerequisites

MemoryRelay tools must be available in your environment via one of:

- **[MemoryRelay MCP server](https://github.com/memoryrelay/mcp-server)** — for Claude Code, Cursor, or any MCP-compatible client
- **[OpenClaw plugin](https://github.com/memoryrelay/openclaw-plugin)** — for OpenClaw agents

## Usage

Skills are invoked automatically when your task matches their description. You can also invoke them explicitly:

- `/memory-workflow` — Follow the full session lifecycle
- `/decision-tracking` — Record or check architectural decisions
- `/pattern-management` — Create or search reusable patterns
- `/project-orchestration` — Load context and analyze impact
- `/entity-and-context` — Build and traverse knowledge graphs

## Links

- [MemoryRelay](https://memoryrelay.com)
- [MCP Server](https://github.com/memoryrelay/mcp-server)
- [OpenClaw Plugin](https://github.com/memoryrelay/openclaw-plugin)

## License

MIT

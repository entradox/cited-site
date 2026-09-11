# cited-site

Cited — does AI recommend your practice? Instant free scan, verbatim evidence.

**Live:** offer page at https://entradox.github.io/cited-site/ · API at https://cited-api-production.up.railway.app/health · MCP at https://cited-api-production.up.railway.app/mcp/

## Connect Cited (agents are first-class citizens)

No OAuth, no signup — one POST scans any business instantly.

**Claude Code:**
```bash
claude mcp add --transport http cited https://cited-api-production.up.railway.app/mcp/
```

**Codex:**
```bash
codex mcp add cited --url https://cited-api-production.up.railway.app/mcp/
```

**Cursor** — merge into `mcp.json`:
```json
{ "mcpServers": { "cited": { "url": "https://cited-api-production.up.railway.app/mcp/" } } }
```

**Any MCP client:** point it at the streamable-http remote above. **REST:** `POST /scan`, `GET /report/{id}` — API reference for agents: https://cited-api-production.up.railway.app/llms.txt

**Try these prompts once connected:**
- "Scan Gentry Dentistry of Suwanee for AI visibility"
- "Is my dental practice recommended by AI engines?"

Operated by the Cited API (Railway). Terms: https://entradox.github.io/cited-site/terms.html

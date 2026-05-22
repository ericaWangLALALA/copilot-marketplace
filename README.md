# Company Copilot Plugin

A reusable enterprise plugin package for GitHub Copilot. It bundles:

- Shared skills
- Project instructions
- Agent personas
- Local hooks
- MCP server config

## Install In Any Project

```bash
copilot plugin install ericaWangLALALA/copilot-marketplace
```

Or if published to a registry/alias:

```bash
copilot plugin install your-org/company-copilot-plugin
```

## Structure

```text
.
├── plugin.json
├── README.md
├── skills/
│   ├── backend-review/
│   │   └── SKILL.md
│   ├── react-architecture/
│   │   └── SKILL.md
│   └── kubernetes-debug/
│       └── SKILL.md
├── instructions/
│   └── coding.instructions.md
├── hooks/
│   └── pre-commit.sh
├── mcp/
│   └── servers.json
└── agents/
    └── senior-reviewer.md
```

## Example Usage

- "Use backend-review skill to review this PR"
- "Use senior-reviewer agent to do a risk-first review"
- "Follow coding.instructions.md for this repo"

## Notes

- Repository URL is set to `https://github.com/ericaWangLALALA/copilot-marketplace`.
- Prefer `owner/repo` install over full URL for a shorter command namespace.
- Update `mcp/servers.json` with your real MCP server command.
- Keep skills small and composable.

# onbangdan

Claude Code project setup: frontend design skills, animation skill, and MCP servers for browser + Figma access.

## Installed skills (`.claude/skills`, symlinked from `.agents/skills`)

| Skill | Source | What it does |
| --- | --- | --- |
| `frontend-design` | [anthropics/skills](https://github.com/anthropics/skills) | Aesthetic direction and typography guidance so UI doesn't read as templated defaults. |
| `design-taste-frontend` | [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) | Tunable dials for design variance, motion intensity, and visual density. |
| `animate` | [OneWave-AI/claude-skills](https://github.com/OneWave-AI/claude-skills) | Generates Framer Motion animations/motion graphics from natural language. |

Skill versions are pinned in `skills-lock.json`. Update with `npx skills update`.

## MCP servers (`.mcp.json`, project-scoped)

- **playwright** — `npx @playwright/mcp@latest`, browser automation/testing.
- **figma-dev-mode-mcp-server** — SSE connection to a local Figma Dev Mode MCP server (`http://127.0.0.1:3845/sse`). Requires the Figma desktop app running in Dev Mode with a Dev or Full seat.

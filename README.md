# MCP Developer Workflows & Starter Prompts

An open-source repository providing ready-to-use **Model Context Protocol (MCP)** configurations, automated code review templates, and debugging prompts for open-source maintainers.

## 🚀 Features
- **Automated PR Review Prompts:** Standardized system prompts for evaluating code quality and security.
- **MCP Server Configs:** Example JSON configurations for connecting local tools (Git, SQLite, Filesystem) to LLMs.
- **Issue Triage Templates:** Structured prompts for reproducing and fixing open-source bugs.

## 📦 Example MCP Configuration (`claude_desktop_config.json`)
```json
{
  "mcpServers": {
    "filesystem": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-filesystem", "./workspace"]
    },
    "github": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-github"]
    }
  }
}

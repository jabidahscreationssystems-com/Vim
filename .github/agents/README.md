# GitHub Copilot Custom Agents for VSCodeVim

This directory contains custom agent configurations for GitHub Copilot to help with development of the VSCodeVim extension.

## Available Agents

### vscodevim-dev.agent.md

The main development agent for VSCodeVim. This agent is an expert in:
- Vim behavior and command implementation
- TypeScript and VS Code extension API
- VSCodeVim codebase architecture and patterns
- MCP (Model Context Protocol) server integration
- Playwright browser automation
- Remote tunnel VS Code development

**Usage:** This agent is configured with `infer: true`, so it will automatically activate when working on VSCodeVim-related tasks. You can also manually select it when needed.

**Capabilities:**
- Code reading and editing
- Repository search
- Running build and test commands
- Understanding Vim emulation patterns
- MCP server integration for enhanced workflows
- Playwright automation for E2E testing
- Remote development environment support

## Enhanced Features

### MCP Server Integration

The agent supports Model Context Protocol (MCP) servers for:
- Enhanced context awareness
- Integration with external tools
- Automated workflows and testing
- Access to repository metadata

**Setup:** Create `.vscode/mcp.json` with appropriate server configurations (see agent file for examples).

### Playwright Browser Automation

Playwright MCP integration enables:
- Automated UI testing
- E2E test generation
- Browser-based debugging
- Visual regression testing

**Setup:** Install `@playwright/mcp` and configure in your MCP settings.

### Remote Tunnel Support

The agent works seamlessly with VS Code Remote Tunnels:
- Full agent capabilities in remote environments
- MCP servers run on remote machines
- Playwright tests execute remotely
- Consistent development experience

**Security Features:**
- **Git Guardian** - Automated secret scanning and prevention
- **Health Sentinel** - Invisible background monitoring of tunnel health
- **Stealth Sentry** - Real-time threat detection and security enforcement
- Automated security auditing and compliance
- Encrypted connections with multi-factor authentication

**Setup:** Use `code tunnel` to start a remote development session with built-in security monitoring.

## Configuration

The agent configuration follows GitHub's custom agent specification:
- YAML frontmatter defines agent metadata
- Markdown body provides detailed instructions and context
- Based on existing `.github/copilot-instructions.md` but enhanced for agent use
- Extended with MCP, Playwright, and remote tunnel documentation

## References

- [GitHub Copilot Custom Agents Documentation](https://docs.github.com/en/copilot/how-tos/use-copilot-agents/coding-agent/create-custom-agents)
- [Custom Agents Configuration Reference](https://docs.github.com/en/copilot/reference/custom-agents-configuration)
- [Model Context Protocol (MCP)](https://docs.github.com/en/copilot/how-tos/use-copilot-agents/coding-agent/extend-coding-agent-with-mcp)
- [Playwright MCP Server](https://www.npmjs.com/package/@playwright/mcp)
- [VS Code Remote Tunnels](https://code.visualstudio.com/docs/remote/tunnels)
- [GitGuardian - Secret Scanning](https://www.gitguardian.com/)



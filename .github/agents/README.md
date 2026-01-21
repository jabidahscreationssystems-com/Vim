# GitHub Copilot Custom Agents for VSCodeVim

This directory contains custom agent configurations for GitHub Copilot to help with development of the VSCodeVim extension.

## Available Agents

### vscodevim-dev.agent.md

The main development agent for VSCodeVim. This agent is an expert in:
- Vim behavior and command implementation
- TypeScript and VS Code extension API
- VSCodeVim codebase architecture and patterns

**Usage:** This agent is configured with `infer: true`, so it will automatically activate when working on VSCodeVim-related tasks. You can also manually select it when needed.

**Capabilities:**
- Code reading and editing
- Repository search
- Running build and test commands
- Understanding Vim emulation patterns

## Configuration

The agent configuration follows GitHub's custom agent specification:
- YAML frontmatter defines agent metadata
- Markdown body provides detailed instructions and context
- Based on existing `.github/copilot-instructions.md` but enhanced for agent use

## References

- [GitHub Copilot Custom Agents Documentation](https://docs.github.com/en/copilot/how-tos/use-copilot-agents/coding-agent/create-custom-agents)
- [Custom Agents Configuration Reference](https://docs.github.com/en/copilot/reference/custom-agents-configuration)

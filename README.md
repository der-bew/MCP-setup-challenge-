# MCP Setup Challenge

This repository captures a minimal MCP (Model Context Protocol) workspace configuration for connecting VS Code to the TenX Feedback Analytics proxy server. Use it as a reference or starting point when wiring up MCP-enabled tools in your own projects.

## Repository Layout
- `.vscode/mcp.json` defines the MCP servers the workspace can reach.
- `.github/copilot-instructions.md` outlines Copilot usage guidance and review expectations.

## Prerequisites
- VS Code with MCP-capable extensions (for example, GitHub Copilot Chat with MCP preview enabled).
- Git to clone and manage the repository.
- Network access to `https://mcppulse.10academy.org/proxy`.

## Getting Started
- Clone the repository: `git clone https://github.com/der-bew/MCP-setup-challenge-.git`
- Open the folder in VS Code.
- Review `.vscode/mcp.json` to confirm the configured server details meet your environment needs.
- Trigger the MCP-enabled assistant (e.g., GitHub Copilot Chat) and verify the `tenxfeedbackanalytics` server appears under the available MCP connections.

## Troubleshooting Tips
- If the server does not appear, ensure the MCP preview feature flag is enabled in your editor.
- Check that the proxy URL is reachable from your network and not blocked by a firewall.
- Restart the MCP client or reload VS Code after making configuration changes.

## Contributing
- Open an issue or pull request with proposed improvements.
- Follow the guidance in `.github/copilot-instructions.md` for maintaining review quality and consistency.
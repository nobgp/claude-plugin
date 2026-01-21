# nobgp Claude Code Plugin

Manage nobgp networks, nodes, and services from Claude Code.

## Installation

```bash
claude plugin install https://github.com/nobgp/claude-plugin
```

## Authentication

After installation, authenticate with nobgp:
```
/mcp
```
Select "nobgp" and complete the OAuth flow in your browser.

## Available Tools

- `network_directory` - List networks, nodes, and services
- `network_create` / `network_delete` - Manage networks
- `register_node` - Generate node registration codes
- `service_publish` / `service_update` / `service_delete` - Manage services
- `tty_exchange` - Interactive shell on remote nodes
- `whoami` - Show authenticated user

## Slash Commands

- `/nobgp:deploy-server` - Guided workflow to set up and expose a webserver

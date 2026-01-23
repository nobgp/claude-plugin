# nobgp Plugin

Manage nobgp networks, nodes, and services from Claude Code.

## Installation

First, add the marketplace:
```bash
claude plugin marketplace add nobgp/claude-plugin
```

Then install the plugin:
```bash
claude plugin install nobgp@nobgp-marketplace
```

## Authentication

After installation, authenticate with nobgp:
```
/mcp
```
Select the nobgp server and complete the OAuth flow in your browser.

## Available Tools

**Networks**
- `network_directory` - List networks, nodes, and services
- `network_create` / `network_delete` - Manage networks

**Nodes**
- `provision_node` - Provision a new cloud node
- `deprovision_node` - Stop and remove a provisioned node
- `register_node` - Generate registration code for self-hosted nodes
- `tty_exchange` - Interactive shell on remote nodes

**Services**
- `service_publish` - Expose a port or command via public URL
- `service_update` / `service_delete` - Manage published services

**Account**
- `whoami` - Show authenticated user info

## Slash Commands

- `/deploy-server` - Guided workflow to set up and expose a webserver on a node

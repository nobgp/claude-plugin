---
name: deploy-server
description: Set up and expose a webserver on a nobgp node
---

Help the user deploy and expose a webserver on a nobgp node.

## Workflow

1. **Show available infrastructure**
   - Use `network_directory` to list networks and nodes
   - Ask which node to use (or accept if specified)

2. **Set up the webserver via TTY**
   - Use `tty_exchange` to connect to the node
   - Help install dependencies if needed
   - Guide through creating/configuring the webserver
   - Start the server process

3. **Expose the service**
   - Use `service_publish` to create a proxy URL
   - Confirm the public URL is accessible

## Guidelines
- Ask for port number, working directory preferences
- Suggest sensible defaults (port 8080, current directory)
- Handle errors gracefully - if tty_exchange fails, explain what went wrong
- After publishing, provide the public URL prominently

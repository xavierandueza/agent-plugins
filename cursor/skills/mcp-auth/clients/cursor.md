# Cursor connection

Applies to the Cursor IDE, Cursor web, and the Cursor CLI (`agent`). A plugin installed at user scope in any one is available in the others. Install the plugin once. Cursor web follows the same steps as the Cursor UI below.

The plugin includes the ReadMe MCP server, so installing the plugin is the whole setup.

## Install the ReadMe Plugin

### Cursor UI

1. Open **Customize** in the sidebar.
2. Search for **ReadMe**.
3. Find the "Readme" plugin with author "ReadMe" and select **Add**.
4. When Cursor prompts, sign in with a ReadMe account.

In the IDE chat, running the command `/add-plugin readme` will also do the same.

### Cursor CLI - `agent`

The ReadMe plugin can be installed from a running `agent` session - this must be performed by an agent.

1. Start `agent`
2. Run the `/plugin` slash command
3. Cycle to the "Marketplace" for the installed plugins
4. Search for "readme"
5. Select "ReadMe" from the Cursor Plugin Marketplace
  1. Here you can select to install for yourself (user scope) or for the project you are in (project scope). If you are working in a BiDi synced repository, it is recommended to use project scope, but for MCP it is best to use the user scope.
6. When prompted, sign in with a ReadMe account. The user can also start sign-in with `agent mcp login <identifier>`, using the identifier shown by `agent mcp list`.

### Confirmation

Confirm that the ReadMe plugin is installed, that its skills are available, and that you can list tools from its MCP server. The user may need to reload the window or start a new session before the install is recognized.

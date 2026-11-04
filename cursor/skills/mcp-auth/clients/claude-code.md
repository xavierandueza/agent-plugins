# Claude Code connection

Applies to the Claude Code CLI and the Code tab in the Claude Desktop App. For claude code cloud agents, the Chat interface in the Claude Desktop App or claude.ai refer to `./claude-chat.md` instead.

These commands can be run by Claude Code (in either the CLI or the desktop app), or the user can run them manually.

## Install the ReadMe Plugin

You must add the ReadMe plugin marketplace from the official agent-plugins repository, then install the plugin from that marketplace.

### User scope (Recommended)

Available to the user in every project.

```sh
claude plugin marketplace add https://github.com/xavierandueza/agent-plugins.git
claude plugin install readme@readme --scope user
```

### Project scope

Recommended if the user is working in a BiDi synced repository. The plugin is enabled in the project's `.claude/settings.json`, which is committed so that other contributors are prompted to install it.

```sh
claude plugin marketplace add https://github.com/readmeio/agent-plugins.git --scope project
claude plugin install readme@readme --scope project
```

Nothing secret is committed. Each contributor signs in with their own ReadMe account.

### Confirmation

That you are able to successfully read skills from the installed ReadMe plugin.

## Sign in

The plugin includes the ReadMe MCP server. Claude Code prompts the user to sign in with their ReadMe account when ReadMe asks for it. To sign in at any time, the user runs `/mcp`, selects the ReadMe server, and completes sign-in in the browser.


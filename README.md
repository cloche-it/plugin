# Cloche plugin

Cloche lets your agent publish a client-side app and share it with a link.

## Install

Ask your agent to follow the [Cloche setup instructions](https://cloche.dev/agent-setup/prompt.md). It will connect the MCP server and verify the connection.

In Claude Code, add this repository as a marketplace with `/plugin marketplace add cloche-it/plugin`, then install with `/plugin install cloche@cloche`.

In Codex, add the repository with `codex plugin marketplace add cloche-it/plugin`, then install Cloche from `/plugins`.

In other clients that support Agent Plugins, install this repository as a plugin. Complete the browser sign-in. If the tools do not appear, start a new chat.

You can also add `https://mcp.cloche.dev/mcp` as an MCP server. This connects the tools without installing the bundled skill.

## Apps

Cloche hosts HTML, CSS and JavaScript without server code or a build step. The app gets storage and the signed-in viewer through `window.cloche.*`.

## Data and privacy

The plugin is a skill and an MCP server setting. It runs no scripts or hooks. Your agent talks to Cloche's MCP server, `https://mcp.cloche.dev/mcp`. Images and other binary files may go to a Cloche upload address that server returns. The agent sends:

- The app: its files, name, address, icon and data schema, and a line on what it is for or what changed.
- With every publish, and when it saves unfinished work, a note of up to 16 KB so another chat can pick it up. It covers the goal, where the work stands, decisions, what is left, checks run and known issues. The tools tell the agent to leave out the chat transcript, credentials and the data people saved in the app.
- When you share an app, the email address or name of each person you invite.
- When an app shows data from another connected service, the read-only calls that fetch it: the service's address and label, the tool names and their arguments, and a line on what you chose to share. Cloche makes those calls with each viewer's own access when the app is read. If the owner keeps a copy for people without access, Cloche makes them with the owner's access and stores the result.

See the [privacy policy](https://cloche.dev/privacy/).

## Support

hi@cloche.dev

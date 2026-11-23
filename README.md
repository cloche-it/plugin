# Cloche plugin

Cloche lets your agent publish a client-side app and share it with a link.

## Install

Ask your agent to follow the [Cloche setup instructions](https://cloche.dev/agent-setup/prompt.md). It will connect the MCP server and verify the connection.

In Claude Code, add this repository as a marketplace with `/plugin marketplace add cloche-it/plugin`, then install with `/plugin install cloche@cloche`.

In Codex, add the repository with `codex plugin marketplace add cloche-it/plugin`, then install Cloche from `/plugins`.

In other clients that support Agent Plugins, install this repository as a plugin. Complete the browser sign-in. If the tools do not appear, start a new chat.

You can also add `https://mcp.cloche.dev/mcp` as an MCP server. This connects the tools without installing the bundled skill.

## Data and privacy

The plugin is a skill and an MCP server setting. It runs no scripts or hooks. Your agent talks to Cloche's MCP server, `https://mcp.cloche.dev/mcp`. Images and other binary files may go to a Cloche upload address that server returns. The agent sends:

- The app: its files, name, address, icon and data schema, and a line on what it is for or what changed.
- A short note on the work, so another chat can pick it up. The tools tell the agent to leave out the chat transcript, credentials and the data people saved in the app.
- When you share an app, the email address or name of each person you invite.
- When an app needs data from another service, the service's name or address and a line on the data it needs. For a company database, the agent may also suggest one table, its columns, filters and changes, never a statement. Cloche sends you a link, and you pick the exact data on a Cloche page. Nothing is read before you choose. Each time the app loads that data, Cloche makes the calls you picked with the viewer's own access. If the owner keeps a copy instead, Cloche makes the calls with the owner's access, stores the result and shows that copy to everyone who can open the app.
- When you add or change an app's records, the fields you send.

See the [privacy policy](https://cloche.dev/privacy/).

## Support

hi@cloche.dev

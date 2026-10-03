# Cloche plugin

Cloche lets your agent publish a client-side app and share it with a link.

## Install

Ask your agent to follow the [Cloche setup instructions](https://cloche.dev/agent-setup/prompt.md). It will connect the MCP server and verify the connection.

In Claude Code, add this repository as a marketplace with `/plugin marketplace add cloche-it/plugin`, then install with `/plugin install cloche@cloche`.

In Codex, add the repository with `codex plugin marketplace add cloche-it/plugin`, then install Cloche from `/plugins`.

In Gemini CLI, install with `gemini extensions install https://github.com/cloche-it/plugin`. Then start `gemini` and run `/mcp auth cloche` to sign in.

In other clients that support Agent Plugins, install this repository as a plugin. Complete the browser sign-in. If the tools do not appear, start a new chat.

You can also add `https://mcp.cloche.dev/mcp` as an MCP server. This connects the tools without installing the bundled skill.

## Data and privacy

The plugin is a skill and an MCP server setting. It runs no scripts or hooks. Your agent talks to Cloche's MCP server, `https://mcp.cloche.dev/mcp`. Images and other binary files may go to a Cloche upload address that server returns. The agent sends:

- The app: its files, name, address, icon and data schema, and a line on what it is for or what changed.
- A short note on the work, so another chat can pick it up. The tools tell the agent to leave out the chat transcript, credentials and the data people saved in the app.
- When you share an app, the email address or name of each person you invite.
- When an app shows data from another connected service, the read-only calls that fetch it: the service's address and label, the tool names and their arguments, and a line on what you chose to share. Each time the app loads that data, Cloche makes those calls with the viewer's own access. If the owner keeps a copy instead, Cloche makes the calls with the owner's access, stores the result and shows that copy to everyone who can open the app.

See the [privacy policy](https://cloche.dev/privacy/).

## Support

hi@cloche.dev

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

## Support

hi@cloche.dev

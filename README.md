# Cloche plugin

**Your AI App. Served.** This plugin connects your agent to [Cloche](https://cloche.dev), a home for the apps people make with AI agents. Build an app in the chat, publish it with one call, and share it with a link.

One repo carries the manifest for each host. They all point at the same address, `https://mcp.cloche.dev/mcp`, and the same skill. Sign-in happens in the browser; there are no keys or headers to paste. Access is not open to everyone yet. Someone new may be asked to join the Cloche waitlist when they sign in, and an agent cannot approve that for them.

## Cursor and Grok Bot

1. Install **Cloche** from the marketplace (Cursor: Customize; Grok Bot: Settings, then Plugins).
2. Sign in when your browser opens, then switch back if it does not bring you back. Sign-in can land on the waitlist; an agent cannot approve that.
3. Start a new chat. In Grok Bot, type `@` and pick Cloche when you give a Bot a task.

## Claude Code

1. Install **Cloche** from the plugin directory, or add this repo as a marketplace and install from it.
2. Sign in when your browser opens. Sign-in can land on the waitlist; an agent cannot approve that.
3. Start a new chat.

## Codex

1. Install **Cloche** from the plugin directory.
2. Sign in when your browser opens. Sign-in can land on the waitlist; an agent cannot approve that.
3. Start a new chat.

## Adding it by hand

Every host also takes the address directly: add a connector at `https://mcp.cloche.dev/mcp`, sign in when the browser opens, and start a new chat. Sign-in can land on the waitlist; an agent cannot approve that.

## What it gives your agent

- The Cloche tools: publish an app, check its status, set who can open it, save and resume work, list and delete apps.
- A skill that tells the agent to read the current Cloche contract before its first publish, so it builds the right shape of app.

## What an app looks like

One self-contained page: HTML, CSS and JavaScript, no server code and no build step. Storage and the signed-in viewer come from `window.cloche.*`; the platform scopes rows to the person looking. The full contract lives at [cloche.dev/agent-setup/prompt.md](https://cloche.dev/agent-setup/prompt.md).

## Support

hi@cloche.dev

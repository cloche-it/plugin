# Cloche for Cursor and Grok Bot

**Your AI App. Served.** This plugin connects Cursor and Grok Bot to
[Cloche](https://cloche.dev), a home for the apps people make with AI agents.
Build an app in the chat, publish it with one call, and share it with a link.

## Install

Install **Cloche** from the marketplace, then connect the `cloche` server. A
browser window opens for sign-in; that is the whole account.

Or add it by hand: the server address is `https://mcp.cloche.dev/mcp`. It
needs no keys or headers. Sign-in happens in the browser.

## What it gives your agent

- The Cloche tools: publish an app, check its status, set who can open it,
  save unfinished work, and pick an app back up later.
- A skill that tells the agent to read the current Cloche contract before its
  first publish, so it builds the right shape of app.

## What an app looks like

One self-contained page: HTML, CSS and JavaScript, up to 256 KB, no server
code and no build step. Storage and the signed-in viewer come from
`window.cloche.*`; the platform scopes rows to the person looking. The full
contract lives at [cloche.dev/agent-setup](https://cloche.dev/agent-setup).

## Support

hi@cloche.dev

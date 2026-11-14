# Awesome Agent Email [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Tools, MCP servers and guides for giving AI agents email: their own inbox, or access to yours.

AI agents need email to sign up for services, read verification codes, receive invoices and reply to people. There are two ways to do it, and they suit different jobs:

- **Give the agent its own inbox.** A hosted inbox the agent controls through an API, MCP or a CLI. Best for sign-ups, verification codes and errands that shouldn't touch your personal mail.
- **Give the agent access to your inbox.** An MCP server for Gmail, Outlook or any IMAP account. Best when you want the agent to work on your own email.

This list is maintained by [Replyz](https://replyz.io), which makes one of the products listed. Entries are sorted alphabetically within each section, and each one is checked by hand. Pull requests are welcome; see [contributing](CONTRIBUTING.md).

## Contents

- [Hosted inboxes for agents](#hosted-inboxes-for-agents)
- [MCP servers for agent inboxes](#mcp-servers-for-agent-inboxes)
- [MCP servers for your own mailbox](#mcp-servers-for-your-own-mailbox)
- [Agent integrations](#agent-integrations)
- [Guides](#guides)
- [Related lists](#related-lists)

## Hosted inboxes for agents

Services that give each agent an email address of its own.

- [AgentMail](https://www.agentmail.to) - API-first inboxes for AI agents, with an MCP server, a CLI, SDKs and agent self-signup.
- [Dead Simple Email](https://deadsimple.email) - Inboxes with IMAP/SMTP credentials, an API, SDKs, a CLI and an MCP server; parses verification codes.
- [Nylas agent accounts](https://www.nylas.com) - An email inbox and calendar for an agent, hosted by Nylas, with US or EU hosting.
- [Replyz](https://replyz.io) - EU-hosted inboxes for personal agents (OpenClaw, Hermes, Claude Code) with wait-for-email and code extraction; in private early access.
- [Resend Inboxes](https://resend.com) - Inboxes inside the Resend email API; received mail counts toward the sending quota.

## MCP servers for agent inboxes

- [agentmail-to/agentmail-mcp](https://github.com/agentmail-to/agentmail-mcp) - Official AgentMail MCP server.
- [resend/resend-mcp](https://github.com/resend/resend-mcp) - Official Resend MCP server for sending email and working with Resend.

## MCP servers for your own mailbox

These connect an agent to an existing account. The agent can read and send as you, so scope the access carefully.

### IMAP and SMTP (any provider)

- [codefuturist/email-mcp](https://github.com/codefuturist/email-mcp) - IMAP and SMTP: read, search, send and manage mail.
- [mehdis34/fezola-mcp](https://github.com/mehdis34/fezola-mcp) - Hosted remote MCP server for Gmail, Outlook, iCloud and any IMAP mailbox, plus Google Chat, Telegram, Calendar, Notion, Search Console, Cloudflare, PostHog, a shared Memory and ad platforms (Google Ads, Microsoft Advertising, OpenAI Ads): read, search and draft replies across all your inboxes (drafts by default, direct sending only if you enable it).
- [nikolausm/imap-mcp-server](https://github.com/nikolausm/imap-mcp-server) - IMAP and SMTP for AI assistants: search, read, send and organise.

### Gmail and Google Workspace

- [shinzo-labs/gmail-mcp](https://github.com/shinzo-labs/gmail-mcp) - MCP server for the Gmail API.
- [taylorwilsdon/google_workspace_mcp](https://github.com/taylorwilsdon/google_workspace_mcp) - Gmail, Calendar, Docs, Sheets and more through one MCP server.

### Outlook and Microsoft 365

- [ryaker/outlook-mcp](https://github.com/ryaker/outlook-mcp) - Outlook mail and calendar through Microsoft Graph.

## Agent integrations

- [mvanhorn/agentmail-to-claude-code](https://github.com/mvanhorn/agentmail-to-claude-code) - Opens a Claude Code session for each inbound AgentMail message.

## Guides

- [Custom connectors with remote MCP (Claude)](https://support.claude.com/en/articles/11175166-getting-started-with-custom-connectors-using-remote-mcp) - Adding a remote MCP server to Claude, including request headers for API keys.
- [Cursor MCP configuration](https://cursor.com/docs/context/mcp) - `mcp.json`, remote servers and environment variables in headers.
- [Hermes Agent messaging](https://hermes-agent.nousresearch.com/docs/user-guide/messaging/) - Hermes gateways, including email.
- [Give OpenClaw its own email inbox](https://replyz.io/openclaw) - Skill-based setup, and why not to connect your Gmail.
- [Gmail MCP server vs an agent inbox](https://replyz.io/gmail-mcp-alternative) - When to give the agent your inbox, and when to give it its own.

## Related lists

- [awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) - MCP servers of every kind.
- [awesome-openclaw-skills](https://github.com/VoltAgent/awesome-openclaw-skills) - Skills for OpenClaw.
- [awesome-hermes-agent](https://github.com/0xNyk/awesome-hermes-agent) - Skills, tools and integrations for Hermes Agent.
- [awesome-claude-code](https://github.com/hesreallyhim/awesome-claude-code) - Resources for Claude Code.

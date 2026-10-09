# BugTape plugins

Bug evidence for your coding agent. Connect a workspace, choose a project, and investigate a real failure.

This public repository contains the BugTape plugin and marketplace files for Claude Code, Codex and Grok Build. It connects to the hosted MCP server at `https://app.bugtape.ai/mcp`. Sign in through your host's connection flow. New users can create a free BugTape workspace during sign-in.

## Install

### Claude Code

```sh
claude plugin marketplace add jackfieldman/bugtape-plugins
claude plugin install bugtape@bugtape-plugins
```

Open `/mcp`, select BugTape and sign in. Then run `/bugtape:setup`.

### Codex

```sh
codex plugin marketplace add https://github.com/jackfieldman/bugtape-plugins.git
codex plugin add bugtape@bugtape-plugins
```

Open BugTape in Plugins and complete the connection. Start a fresh conversation if the skills do not appear.

### Grok Build

```sh
grok plugin marketplace add jackfieldman/bugtape-plugins
grok plugin install bugtape@bugtape-plugins
```

Review the plugin trust prompt to finish installation. Complete the host's MCP sign-in flow, then ask: “Connect BugTape and choose my project.”

## Use it

- **Setup:** choose the workspace and project before reading bugs.
- **Triage:** read one failure and explain the captured evidence and gaps.
- **Report:** file an observed failure when asked.
- **Verify:** check a verification receipt. A pull request alone is not proof of a fix.

Try: “Find the most urgent BugTape issue in my chosen project. Explain the evidence and the next step.”

For Claude chat, ChatGPT and Grok chat, use the [chat connection guide](https://bugtape.ai/docs/plugins/#chat-apps). A custom MCP connection supplies tools; the bundled skills require a plugin installation. This repository is an install source, not a claim of directory approval.

## Access and cost

You choose the workspace, permissions and access duration. You can revoke agent access in the BugTape console. No credentials, executable hooks or background polling service are bundled.

MCP works on every BugTape plan. On Free and Prepaid, reading captured events costs 2 credits; other reads are free. Pro includes event reads. Do not paste passwords or tokens into a chat to install the plugin.

## Release 0.1.0

The files under `plugins/bugtape` and both marketplace manifests match the reviewed [0.1.0 marketplace download](https://bugtape.ai/plugins/bugtape-marketplace-0.1.0.zip). [Release hashes](./release.json) are also available [on BugTape](https://bugtape.ai/plugins/release.json).

The unchanged 0.1.0 plugin README describes its original private source. This repository is the standalone public distribution it mentions. Product implementation remains in a separate private repository.

## Help

[Install guide](https://bugtape.ai/docs/plugins/) · [Quickstart](https://bugtape.ai/docs/quickstart/) · [Support](https://bugtape.ai/contact/) · [Privacy](https://bugtape.ai/privacy/) · [Terms](https://bugtape.ai/terms/)

Apache-2.0. See [LICENSE](./LICENSE).

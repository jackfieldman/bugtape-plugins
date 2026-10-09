# BugTape

Production bug evidence for people who build with coding agents. This plugin connects to BugTape's hosted MCP server. It helps you choose a workspace and project, investigate a failure, file an observed bug when asked, and check the proof of a fix.

The bundle contains four short workflows: setup, triage, report and verify. It uses native OAuth sign-in. No token, password, capture key, executable hook or background polling service is bundled. New users can create a free workspace during sign-in, then choose what the agent can access.

## Start here

Install instructions for Claude Code, Codex, Grok Build and their chat apps are at [BugTape plugins](https://bugtape.ai/docs/plugins/). Directory availability varies by platform. A downloadable package does not imply public directory approval.

After connecting, ask: “Connect BugTape and choose my project.” Then ask: “Find the most urgent BugTape issue in this project and explain the evidence.”

## Access and cost

You choose the workspace, permissions and access duration. Capture keys cannot authenticate MCP. On Free and Prepaid, captured-event reads use credits; Pro includes those reads. The agent should read only relevant evidence. A pull request is a proposed fix; a verification receipt is separate evidence.

## Help

[Documentation](https://bugtape.ai/docs/plugins/) · [Support](https://bugtape.ai/contact/) · [Privacy](https://bugtape.ai/privacy/) · [Terms](https://bugtape.ai/terms/)

Licensed under Apache-2.0. See LICENSE.

## Local marketplace install

Unzip the marketplace download and run `claude plugin marketplace add ./bugtape-plugins`, then `claude plugin install bugtape@bugtape-plugins`. The same download works with Codex and Grok Build; the docs show each host's commands. The source repository is private. No public repository install is advertised until a standalone distribution is published.

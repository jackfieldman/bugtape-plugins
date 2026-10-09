---
name: setup
description: Connect BugTape, select a workspace and project, and help a new user reach their first useful bug report.
---

# BugTape setup

1. Use the bundled BugTape MCP connection. If it needs authentication, ask the host to start its native sign-in flow. A new user can choose Create one on BugTape's sign-in page. They must approve access after signup. Never ask for a password, PAT or capture key in chat.
2. Call get_current_org and list_projects. State the workspace. Ask for a project if more than one fits. Keep the chosen project ID for this conversation; do not silently use all projects.
3. Ask whether capture is already installed. If yes, help inspect the first report. If not, open https://bugtape.ai/docs/quickstart/ and guide the app's platform. Use setup_capture only when the user asks you to create capture setup and the grant permits it. Do not print or store credentials in the conversation.
4. Give one useful next prompt: “Find the most urgent BugTape issue in this project and explain the evidence.” Say when there are no reports and give the next test-event step.
5. Keep setup short. On Free and Prepaid, reads of captured events cost credits; Pro includes them. A capture key is not an MCP credential. Access denied is a scope or workspace choice to fix with the person, never a reason to widen access yourself.

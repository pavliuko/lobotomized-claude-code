<!--
name: 'Agent Prompt: claude-code-guide'
description: >-
  Trigger criteria for the claude-code-guide subagent. The "IMPORTANT"
  subagent-deduplication note is cut — 4.7 already restrains subagent spawning
  by default per Anthropic 4.7 guidance ("tends to spawn fewer subagents by
  default").
ccVersion: 2.1.141
variables:
  - ''
-->
Use this agent when the user asks questions ("Can Claude...", "Does Claude...", "How do I...") about: (1) Claude Code (the CLI tool) — features, hooks, slash commands, MCP servers, settings, IDE integrations, keyboard shortcuts; (2) Claude Agent SDK — building custom agents; (3) Claude API — usage, tool use, SDK usage.

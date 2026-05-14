<!--
name: MCP per-server instruction router
description: >-
  Patches CC's MCP instruction assembly to consult
  ~/.tweakcc/system-reminders/mcp-<server-name>.md at runtime. Empty body in
  that file drops the server's block. Body containing {{server_instructions}}
  resolves to the server's pristine instructions. Custom body replaces. THIS .md
  does nothing on its own — it just enables per-server .md files. Empty body =
  disable this routing (servers use pristine instructions verbatim).
ccVersion: 2.1.141
-->
This file is a marker that enables per-MCP-server overrides. Edit per-server content in mcp-<server-name>.md alongside this file. Leave this file with content (any content) to enable routing; empty it to disable.

<!--
name: 'MCP server: openaiDeveloperDocs'
description: >-
  Instructions block content for MCP server "openaiDeveloperDocs".
  {{server_instructions}} expands at runtime to the server's pristine
  instructions. Empty body drops the server's block from the model's context.
  Custom body replaces it.
ccVersion: 2.1.141
placeholders:
  - server_instructions
-->
{{server_instructions}}

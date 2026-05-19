<!--
name: Tool-called preamble
description: >-
  Per-tool-call preamble: "Called the X tool with the following input: ...".
  Empty .md body = no preamble (LW strips empty content).
ccVersion: 2.1.141
placeholders:
  - tool_name
  - tool_input
-->
Called the {{tool_name}} tool with the following input: {{tool_input}}

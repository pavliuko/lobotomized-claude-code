<!--
name: Tool-result wrapper
description: >-
  Per-tool-call result wrapper: "Result of calling the X tool: <output>". Empty
  .md body = strip the wrapper line (just emit the result).
ccVersion: 2.1.141
placeholders:
  - tool_name
  - result
-->
Result of calling the {{tool_name}} tool:
{{result}}

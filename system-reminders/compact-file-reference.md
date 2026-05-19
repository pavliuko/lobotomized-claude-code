<!--
name: Compact-time file reference note
description: >-
  Note injected after compaction when a referenced file is too large to inline.
  Conditional. Empty .md body = silent omission.
ccVersion: 2.1.141
placeholders:
  - filename
  - read_tool_name
shadows:
  - system-reminder-compact-file-reference
-->
{{filename}} (read pre-compaction, too large to inline). Use {{read_tool_name}} if needed.

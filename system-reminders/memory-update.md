<!--
name: Memory-update reminder
description: >-
  Fires after dream / consolidation writes new memory files. Conditional. Empty
  .md body = silent updates.
ccVersion: 2.1.141
placeholders:
  - source
  - summary
  - paths
  - in_context_paths
-->
{{source}} memory update: {{summary}}. Files: {{paths}}. Stale in context: {{in_context_paths}}.

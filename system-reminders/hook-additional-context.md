<!--
name: Hook additional-context wrapper
description: >-
  Wraps content returned by user-defined hooks into the model context.
  Conditional. Empty .md body = hook content suppressed.
ccVersion: 2.1.141
placeholders:
  - hook_name
  - hook_content
-->
{{hook_name}} hook additional context: {{hook_content}}

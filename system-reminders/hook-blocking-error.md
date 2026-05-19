<!--
name: Hook blocking-error wrapper
description: >-
  Surfaces hook command failures that block CC continuing. Conditional. Empty
  .md body = errors silenced (DANGEROUS — model will not see why hook blocked).
ccVersion: 2.1.141
placeholders:
  - hook_name
  - command
  - error
-->
{{hook_name}} hook blocking error from command: "{{command}}": {{error}}

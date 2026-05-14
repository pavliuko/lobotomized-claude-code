<!--
name: Edited-text-file post-edit note
description: >-
  Conditional note injected after a file is edited (by user or linter). Empty
  .md body = silent edits.
ccVersion: 2.1.141
placeholders:
  - filename
  - snippet
-->
{{filename}} changed externally — don't revert unless asked:
{{snippet}}

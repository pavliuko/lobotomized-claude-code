<!--
name: 'Tool Description: TaskList'
description: >-
  Empty body suppresses the always-on TaskList description. Inline-blob
  (`inline-tool-task-list.md`) already trims the array form; this empty .md
  prevents `syncPrompt` from auto-recreating pristine and keeps the wipe stable.
  "Could not find" on apply is expected — inline-blob has consumed the array
  before this patch runs.
ccVersion: 2.1.141
variables:
  - ''
-->


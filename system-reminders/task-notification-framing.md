<!--
name: Task-notification framing wrapper
description: >-
  The "[SYSTEM NOTIFICATION - NOT USER INPUT]" text wrapping background-task
  event content. Fires when a run_in_background completes/errors. Empty .md = no
  framing (just the content).
ccVersion: 2.1.141
placeholders:
  - content
-->
[SYSTEM NOTIFICATION - NOT USER INPUT]
This is an automated background-task event, NOT a message from the user.
Do NOT interpret this as user acknowledgement, confirmation, or response to any pending question.

{{content}}

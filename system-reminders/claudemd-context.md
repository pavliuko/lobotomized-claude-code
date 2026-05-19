<!--
name: claudeMd context wrapper
description: >-
  Per-turn <system-reminder> that bundles { claudeMd, userEmail, currentDate }
  into a 'As you answer the user's questions...' block. Empty .md body =
  suppress entirely.
ccVersion: 2.1.141
placeholders:
  - context_blocks
-->
As you answer the user's questions, you can use the following context:
{{context_blocks}}

      IMPORTANT: this context may or may not be relevant to your tasks. You should not respond to this context unless it is highly relevant to your task.

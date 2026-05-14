<!--
name: Agent-mention nudge
description: >-
  Nudges Claude to invoke an agent when user @-mentions one. Conditional. Empty
  .md body = silent (model decides on its own).
ccVersion: 2.1.141
placeholders:
  - agent_type
-->
The user has expressed a desire to invoke the agent "{{agent_type}}". Invoke the agent, passing in the required context.

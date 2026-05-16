<!--
name: 'Agent Prompt: General-purpose (medium variant)'
description: >-
  Phantom variant — cli.js has only one general-purpose source string (1298c at
  JT5 wrapped in `${"..."}` and at oa7 as standalone). The short variant
  overrides the inner 225-char ${"..."} string at oa7; the long variant
  overrides the JT5 outer template literal. There is no separate 402-char source
  for "medium" to bind to, so this override cannot apply independently.
  Lobotomization happens via [[agent-prompt-general-purpose]] which the runtime
  then trims.
ccVersion: 2.1.143
-->


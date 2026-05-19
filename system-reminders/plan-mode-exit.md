<!--
name: Plan-mode exit reminder
description: Fires when leaving plan mode. Conditional. Empty .md body = silent exit.
ccVersion: 2.1.141
placeholders:
  - plan_suffix
shadows:
  - system-reminder-exited-plan-mode
-->
Plan mode exited; edits allowed.{{plan_suffix}}

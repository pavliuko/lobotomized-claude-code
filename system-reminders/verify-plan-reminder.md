<!--
name: Verify-plan reminder
description: >-
  Fires after plan implementation completes, directing Claude to call a
  verification tool. Conditional. Empty .md body = no automatic verification
  nudge.
ccVersion: 2.1.141
placeholders:
  - plan_verifier_tool
shadows:
  - system-reminder-verify-plan-reminder
-->
Plan complete — verify directly (not via {{plan_verifier_tool}} or an agent).

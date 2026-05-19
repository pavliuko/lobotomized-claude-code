<!--
name: Plan-file reference
description: >-
  Surfaces an existing plan file from plan mode. Conditional. Empty .md body =
  plan file invisible to model.
ccVersion: 2.1.141
placeholders:
  - plan_file_path
  - plan_content
shadows:
  - system-reminder-plan-file-reference
-->
Plan at {{plan_file_path}}:
{{plan_content}}

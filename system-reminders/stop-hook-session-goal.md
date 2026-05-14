<!--
name: Stop-hook session-goal reminder
description: >-
  Fires when /goal sets a session-scoped stop hook. Carries the "do not pause to
  ask" framing. Empty .md = silent goal activation (just the condition value
  used internally).
ccVersion: 2.1.141
placeholders:
  - condition
-->
Goal active: "{{condition}}". Acknowledge, then drive it through to completion regardless of task length. Push past obstacles. Don't cut corners, don't quit early, don't wrap up because the work feels long. Stop hook blocks turn-end until the condition holds; auto-clears on success.

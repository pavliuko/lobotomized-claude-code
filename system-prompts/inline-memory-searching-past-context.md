<!--
name: 'Inline blob: searching past context section'
description: >-
  The "## Searching past context" section with grep commands for memory and
  transcript searches.
inlineBlobAnchor: 'return\["## Searching past context"'
inlineBlobKind: array
inlineBlobRawPassthrough: 'true'
injectionGate: memory enabled
ccVersion: 2.1.141
-->
"## Searching past context","","grep memory dir:",`\`grep -rn "term" ${_} --include="*.md"\``,"grep transcripts (slow, last resort):",`\`grep -rn "term" ${q} --include="*.jsonl"\``,"Use narrow terms — error messages, file paths, function names. Broad keywords match too much.",""

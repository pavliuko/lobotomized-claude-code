<!--
name: PDF too-large note
description: >-
  Conditional note when a referenced PDF is too large for direct read. Empty .md
  body = silent omission.
ccVersion: 2.1.141
placeholders:
  - filename
  - page_count
  - file_size
  - read_tool
-->
PDF {{filename}}: {{page_count}} pages, {{file_size}}. Read via {{read_tool}} with `pages: "1-5"` (max 20/request; pages param required).

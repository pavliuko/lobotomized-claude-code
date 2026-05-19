<!--
name: 'MCP server: supabase'
description: >-
  Instructions block content for MCP server "supabase". {{server_instructions}}
  expands at runtime to the server's pristine instructions. Empty body drops the
  server's block from the model's context. Custom body replaces it.
ccVersion: 2.1.141
placeholders:
  - server_instructions
-->
Supabase MCP: read-only + rare one-off edits. Migrations always via Supabase CLI + migration files; never `apply_migration`.
- Schema: `list_tables`
- Debug: `get_logs`, `get_advisors`
- Client config: `get_project_url`, `get_publishable_api_key`

---
description: Verify INSTALL.md matches the Install section of README.md and fix INSTALL.md if it has drifted.
---

Treat `README.md` as the source of truth. `INSTALL.md` exists to host copy-pasteable shell blocks for Install / Update / Remove, and its Install block must stay in sync with the README's Install section.

Do this:

1. Read both `README.md` and `INSTALL.md` at the repo root.
2. Extract the bash block under the README's `## Install` heading and the bash block under the `# Install` heading in `INSTALL.md`.
3. Compare them line-by-line, ignoring:
   - Leading `set -e` in INSTALL.md (the README block doesn't have it; INSTALL.md is a paste-into-shell block where `set -e` is intentional).
   - The `2>/dev/null` vs `2>/dev/null || true` difference on the `mv` lines (INSTALL.md uses `|| true` so `set -e` doesn't abort when the source dir is missing).
4. For every other difference, update `INSTALL.md` to match `README.md`. Do not touch the Update or Remove sections of `INSTALL.md` — only the Install block.
5. If `README.md`'s Install section gains or loses commands (e.g. a new symlink target, a new build step), reflect that in the INSTALL.md Install block while preserving the `set -e` and `|| true` conventions above.
6. Report what you changed, or "INSTALL.md is in sync" if nothing needed updating.

Don't reformat unrelated parts of `INSTALL.md`. Don't update the README — it is the source of truth.

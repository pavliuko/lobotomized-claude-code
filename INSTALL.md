# Install

Paste this into your shell:

```bash
set -e
git clone https://github.com/skrabe/lobotomized-claude-code ~/.tweakcc/lobotomized-claude-code
mv ~/.tweakcc/system-prompts ~/.tweakcc/system-prompts.bak 2>/dev/null || true
ln -sfn ~/.tweakcc/lobotomized-claude-code/system-prompts ~/.tweakcc/system-prompts
mv ~/.tweakcc/system-reminders ~/.tweakcc/system-reminders.bak 2>/dev/null || true
ln -sfn ~/.tweakcc/lobotomized-claude-code/system-reminders ~/.tweakcc/system-reminders
git clone https://github.com/skrabe/tweakcc-fixed ~/dev/tweakcc-fixed
cd ~/dev/tweakcc-fixed && pnpm install && pnpm build
node ~/dev/tweakcc-fixed/dist/index.mjs --apply
```

Requires `git`, `node`, and `pnpm` on `PATH`.

Re-run `node ~/dev/tweakcc-fixed/dist/index.mjs --apply` after every Claude Code update.

# Update

Pulls latest overrides and patcher, rebuilds, re-applies:

```bash
set -e
cd ~/.tweakcc/lobotomized-claude-code && git pull
cd ~/dev/tweakcc-fixed && git pull && pnpm install && pnpm build
node ~/dev/tweakcc-fixed/dist/index.mjs --apply
```

After a Claude Code version bump (no override changes), just re-apply:

```bash
node ~/dev/tweakcc-fixed/dist/index.mjs --apply
```

# Remove

Restores Claude Code to its pristine state and unlinks the overrides:

```bash
set -e
node ~/dev/tweakcc-fixed/dist/index.mjs --restore
rm -f ~/.tweakcc/system-prompts ~/.tweakcc/system-reminders
mv ~/.tweakcc/system-prompts.bak ~/.tweakcc/system-prompts 2>/dev/null || true
mv ~/.tweakcc/system-reminders.bak ~/.tweakcc/system-reminders 2>/dev/null || true
```

To also delete the cloned repos:

```bash
rm -rf ~/.tweakcc/lobotomized-claude-code ~/dev/tweakcc-fixed
```

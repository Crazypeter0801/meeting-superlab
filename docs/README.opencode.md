# Meeting Superlab — OpenCode / Codex-style install

This file is meant to be fetched via a raw GitHub URL for tools that load install instructions from `docs/README.opencode.md`.

## Codex (CLI / App)

```bash
git clone https://github.com/Crazypeter0801/meeting-superlab.git
cd meeting-superlab
codex plugin marketplace add .
```

Then use **`/plugins`** in Codex to install **meeting-superlab** from the **Meeting Superlab** marketplace.

Remote (if supported):

```bash
codex plugin marketplace add Crazypeter0801/meeting-superlab
```

## Cursor

```text
/add-plugin meeting-superlab
```

Or install from disk using the repo root (contains `.cursor-plugin/plugin.json`).

## Claude Code

```text
/plugin marketplace add Crazypeter0801/meeting-superlab
/plugin install meeting-superlab@meeting-superlab-marketplace
```

Full details: [README.md](../README.md) in the repository root.

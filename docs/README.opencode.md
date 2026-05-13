# Meeting Superlab — install from GitHub

**Not on app marketplaces yet.** Install from **https://github.com/Crazypeter0801/meeting-superlab** using the flows below.

This file can be opened via raw GitHub URL for tools that fetch `docs/README.opencode.md`.

## Codex (CLI / App)

```bash
git clone https://github.com/Crazypeter0801/meeting-superlab.git
cd meeting-superlab
codex plugin marketplace add .
```

Then **`/plugins`** → **Meeting Superlab** → install **meeting-superlab**.

Remote (if supported):

```bash
codex plugin marketplace add Crazypeter0801/meeting-superlab
```

## Cursor

1. `git clone https://github.com/Crazypeter0801/meeting-superlab.git`  
2. **Settings → Plugins → Install from disk** → select the repo root (contains `.cursor-plugin/plugin.json`).

## Claude Code

```text
/plugin marketplace add Crazypeter0801/meeting-superlab
/plugin install meeting-superlab@meeting-superlab-marketplace
```

More detail: [README in repo root](https://github.com/Crazypeter0801/meeting-superlab/blob/main/README.md).

# Meeting Superlab

Product-design exploration skills for meeting products: clarification questions, 2–3 options with tradeoffs, need framing, competitor research, insight synthesis, solution exploration, low-fidelity demo prompts, Figma handoff, and structured reviews.

Skills live in `skills/`; reference material in `references/`.

---

## Install: Cursor

**From marketplace (after the repo is listed in the Cursor plugin directory)**

In Cursor Agent chat:

```text
/add-plugin meeting-superlab
```

You can also open **Settings → Plugins** and search for **Meeting Superlab**.

**From a local clone (development)**

1. Clone this repository.  
2. **Settings → Plugins → Install from disk** (or equivalent), and choose the **repository root** (the folder that contains `.cursor-plugin/plugin.json`).

---

## Install: Codex CLI / Codex App

This repo includes **`.agents/plugins/marketplace.json`** for Codex ([plugin build docs](https://developers.openai.com/codex/plugins/build)).

**Clone then add the marketplace locally (recommended)**

```bash
git clone https://github.com/Crazypeter0801/meeting-superlab.git
cd meeting-superlab
codex plugin marketplace add .
```

Then in Codex, open **`/plugins`**, pick the **Meeting Superlab** marketplace, and install **meeting-superlab**.

**Remote marketplace (if your Codex build supports `owner/repo`)**

```bash
codex plugin marketplace add Crazypeter0801/meeting-superlab
```

If remote add fails, use the **local `marketplace add .`** flow above.

---

## Install: Claude Code

```text
/plugin marketplace add Crazypeter0801/meeting-superlab
/plugin install meeting-superlab@meeting-superlab-marketplace
```

- Marketplace manifest: `.claude-plugin/marketplace.json` (`name`: `meeting-superlab-marketplace`).  
- Plugin metadata: `.claude-plugin/plugin.json`.

If your Claude Code build uses different slash commands, use the **Plugins** UI and paste the repository URL.

---

## OpenCode / raw docs

Some setups fetch install notes from GitHub raw URLs. Use:

`https://raw.githubusercontent.com/Crazypeter0801/meeting-superlab/main/docs/README.opencode.md`

---

## Versioning

Keep **the same `version`** in:

- `.cursor-plugin/plugin.json`  
- `.codex-plugin/plugin.json`  
- `.claude-plugin/plugin.json`  
- `.claude-plugin/marketplace.json`  

Currently **0.1.3**.

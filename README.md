# Meeting Superlab

Product-design exploration skills for meeting products: clarification questions, 2–3 options with tradeoffs, need framing, competitor research, insight synthesis, solution exploration, low-fidelity demo prompts, Figma handoff, and structured reviews.

Skills live in `skills/`; reference material in `references/`.

**This plugin is not on the Cursor / vendor marketplaces yet.** The supported path is to **install from this GitHub repository** (clone or add the repo URL / local path in your tool), as below.

Repository: **https://github.com/Crazypeter0801/meeting-superlab**

---

## Install from GitHub: Cursor

1. Clone the repository (or download the ZIP and unzip).

   ```bash
   git clone https://github.com/Crazypeter0801/meeting-superlab.git
   ```

2. In Cursor: **Settings → Plugins → Install from disk** (wording may vary by version).

3. Choose the **repository root folder** — the directory that contains `.cursor-plugin/plugin.json`.

After a future marketplace listing, you may also use **`/add-plugin meeting-superlab`** or search **Meeting Superlab** under Plugins; until then, use the steps above.

---

## Install from GitHub: Codex CLI / Codex App

This repo includes **`.agents/plugins/marketplace.json`** for Codex ([plugin build docs](https://developers.openai.com/codex/plugins/build)).

**Recommended — clone, then register the marketplace from the local folder**

```bash
git clone https://github.com/Crazypeter0801/meeting-superlab.git
cd meeting-superlab
codex plugin marketplace add .
```

Then in Codex, open **`/plugins`**, select the **Meeting Superlab** marketplace, and install **meeting-superlab**.

**Alternative — point Codex at the GitHub repo (if your build supports `owner/repo`)**

```bash
codex plugin marketplace add Crazypeter0801/meeting-superlab
```

If that fails, use the **clone + `marketplace add .`** flow above.

---

## Install from GitHub: Claude Code

```text
/plugin marketplace add Crazypeter0801/meeting-superlab
/plugin install meeting-superlab@meeting-superlab-marketplace
```

- Marketplace manifest: `.claude-plugin/marketplace.json` (`name`: `meeting-superlab-marketplace`).  
- Plugin metadata: `.claude-plugin/plugin.json`.

If slash commands differ in your build, open the **Plugins** UI and add the repository **https://github.com/Crazypeter0801/meeting-superlab**.

---

## OpenCode / raw install notes

Some tools load instructions from a raw GitHub URL:

`https://raw.githubusercontent.com/Crazypeter0801/meeting-superlab/main/docs/README.opencode.md`

---

## Versioning

Keep **the same `version`** in:

- `.cursor-plugin/plugin.json`  
- `.codex-plugin/plugin.json`  
- `.claude-plugin/plugin.json`  
- `.claude-plugin/marketplace.json`  

Currently **0.1.3**.

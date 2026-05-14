# Meeting Superlab

面向会议类产品的设计探索技能：六步 SOP（问题定义 → 竞品研究 → 创意发散 → 取舍收敛 → 低保真 / Figma 交接 → PRD AI Check）及多视角评审；含 `solution-convergence`、`prd-ai-check` 等技能。内容在 `skills/`，参考资料在 `references/`（含 `sop-v0.8.md`）。当前版本 **0.1.4**。

## 安装（只有一个 GitHub 仓库）

**链接（复制给同事即可）：** https://github.com/Crazypeter0801/meeting-superlab

| 工具 | 能不能只靠这个链接安装？ | 怎么做 |
|------|-------------------------|--------|
| **Claude Code** | 可以（用仓库的 `owner/repo`） | `/plugin marketplace add Crazypeter0801/meeting-superlab` → `/plugin install meeting-superlab@meeting-superlab-marketplace` |
| **Codex（App / CLI）** | 多数可以 | `codex plugin marketplace add Crazypeter0801/meeting-superlab`，再在 **`/plugins`** 里安装；若失败则先 `git clone` 再在该目录执行 `codex plugin marketplace add .` |
| **Cursor** | **不能**只打开网页就装完 | 需要先 `git clone`（或下载 ZIP 解压），再在 **Settings → Plugins → Install from disk** 里选**仓库根目录**（里面有 `.cursor-plugin/plugin.json`） |

没有上架应用市场时，**Codex / Claude 用 GitHub 地址即可**；**Cursor 必须先把代码放到本机**，再从磁盘安装。

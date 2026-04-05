# 3devkit — 安装与环境

## OpenSpec

- **CLI**：`openspec --version` 应成功。
- **本机真源（OpenClaw 约定）**：目录 `~/.openclaw/openspec/` 存在。
- **工作目录**：在终端执行时先 **`cd ~/.openclaw`**，再跑 `openspec list`、`openspec status` 等。
- **若缺失**：安装 Node 生态下的 `openspec` CLI；确保 `~/.openclaw/openspec` 被使用或已 `openspec init` 到该路径（以你本机为准）。

## gstack

- **就绪**：`~/.cursor/skills/gstack/setup` 与 `~/.cursor/skills/gstack/VERSION` 存在（完整 clone，而非仅单个 `SKILL.md` 占位）。
- **安装**：
  ```bash
  git clone --depth 1 https://github.com/garrytan/gstack.git ~/.cursor/skills/gstack
  cd ~/.cursor/skills/gstack && ./setup
  ```
- **Slash**：`/office-hours`、`/review` 等需在 **已加载 gstack 的 Claude Code 或 Cursor Agent** 会话中使用。

## Superpowers

- **就绪**：`~/.cursor/skills/using-superpowers/SKILL.md` 存在，或已通过 Cursor **`/add-plugin superpowers`** 安装。
- **备选**：clone `https://github.com/obra/superpowers`，将 `skills/*` 链到 `~/.cursor/skills/`（见 obra 仓库 README）。

## 与 OpenClaw 改造相关的硬规则

修改 **`~/.openclaw/openclaw.json`、多 agent、协议（`AGENTS.md`/`SOUL.md` 等）** 前，必须先走 **OpenSpec change**（见用户 `openclaw-guardrails`）。

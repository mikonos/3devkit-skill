# 3devkit

编排 skill：在 OpenSpec、gstack、Superpowers 三栈之间按产品开发阶段指路；含新手上路、术语表、安装自检与压测用例。

**仓库**：https://github.com/mikonos/3devkit-skill

## 安装（Cursor / 兼容 agentskills 布局）

将目录 `skills/3devkit` 复制到目标机器的：

- **项目内**：`<repo>/.cursor/skills/3devkit/`
- **用户级**：`~/.cursor/skills/3devkit/`

## Agent Skill Hub（已导入）

已通过 **公开 API** 从本仓库导入（无需网页手点）：

- `POST https://agentskillhub.dev/api/v1/repos/analyze` → `POST https://agentskillhub.dev/api/v1/repos/import`
- 技能展示名：**`mikonos/3devkit`**，版本 `2026.04.05`
- 检索：`GET https://agentskillhub.dev/api/v1/search?q=3devkit`

网页提交入口仍可用：[agentskill.sh/submit](https://agentskill.sh/submit)（与 Hub 同源）。

## 许可

MIT — 见 `LICENSE`。

## 上游

开发时可与 `~/.openclaw/openspec`、gstack、`obra/superpowers` 配合使用；本包不捆绑上述项目。

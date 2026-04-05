# 3devkit

编排 skill：在 OpenSpec、gstack、Superpowers 三栈之间按产品开发阶段指路；含新手上路、术语表、安装自检与压测用例。

## 安装（Cursor / 兼容 agentskills 布局）

将目录 `skills/3devkit` 复制到目标机器的：

- **项目内**：`<repo>/.cursor/skills/3devkit/`
- **用户级**：`~/.cursor/skills/3devkit/`

## 提交到目录站（skills / Agent Skill Hub）

1. 本仓库推送到 **公开** GitHub（需你本机登录 GitHub CLI 或网页建库）。
2. 打开 **[agentskill.sh/submit](https://agentskill.sh/submit)**，选 **GitHub Repository**，粘贴仓库 URL，**Analyze & Import**。
3. 可选：[skills.sh](https://skills.sh/) 等目录会索引公开仓库中的 `SKILL.md`；亦可使用各 CLI（如 `npx skillsadd` / `npx skills add`，以各工具当前文档为准）。

## 许可

MIT — 见 `LICENSE`。

## 上游

开发时可与 `~/.openclaw/openspec`、gstack、`obra/superpowers` 配合使用；本包不捆绑上述项目。

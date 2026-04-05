# 3devkit

编排 skill：在 OpenSpec、gstack、Superpowers 三栈之间按产品开发阶段指路；含新手上路、术语表、安装自检与压测用例。

**仓库**：https://github.com/mikonos/3devkit-skill

## 安装

### 方式一：skills CLI（推荐，多 Agent 一次装好）

需已装 Node.js。在**项目根目录**或任意目录执行：

```bash
# 仅当前项目（写入 ./.agents/skills 等，并链到 Cursor / Claude Code 等）
npx skills add mikonos/3devkit-skill -y

# 用户级全局（所有项目可用）
npx skills add mikonos/3devkit-skill -y -g

# 只要 Cursor
npx skills add mikonos/3devkit-skill -y -g -a cursor
```

只装本仓库里这一条 skill 时可用：`--skill 3devkit`（仓库内仅一个 skill 时通常可省略）。

更多选项：`npx skills --help`。发现更多 skill：[skills.sh](https://skills.sh/)。

### 方式二：手动拷贝（纯文件）

把仓库里的目录 **`skills/3devkit`** 整夹复制到：

- **项目内**：`<repo>/.cursor/skills/3devkit/`
- **用户级**：`~/.cursor/skills/3devkit/`

（与 `references/` 子目录一并保留。）

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

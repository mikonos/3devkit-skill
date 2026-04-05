---
name: "3devkit"
description: |
  Use when the user is unsure which of OpenSpec, gstack, or Superpowers to use next;
  wants a phase checkpoint in product work; asks「三栈」「到哪一步」or「3devkit」;
  or needs install hints after tooling checks. Not for deep execution of any single tool.
---

# 3devkit（OpenSpec · gstack · Superpowers）

**默认读者**：不熟悉 OpenSpec / gstack / Superpowers 三栈者 — **首次请先读 `references/onboarding.md`**，术语查 **`references/glossary.md`**。

编排器：**阶段对齐 + 一条下一步 + 缺工具最短安装句**；细则在各工具 SKILL；**openspec-* 的 description 不互链本 skill**。

**When NOT**：已锁定单工具（直跳 `openspec-propose` / `gstack-qa` / `brainstorming`）；要完整执行某条 spec 或整条 gstack 流。

## 环境

OpenSpec：`cd ~/.openclaw`，真源 `~/.openclaw/openspec/`。gstack `/…` 仅在已加载 gstack 的 CC/Cursor Agent 内。详情 **`references/install.md`**。

## 七阶段速查

| # | 阶段 | 优先 |
|---|------|------|
| 1 | 意向 | `/office-hours`；`brainstorming` |
| 2 | 探索 | `/plan-eng-review`；`/plan-design-review`；`openspec list` |
| 3 | 规格 | `openspec new change` + 齐件 + `openspec status`；可选 `/autoplan` |
| 4 | 计划 | `openspec instructions apply`；`writing-plans`、`using-git-worktrees` |
| 5 | 开发 | `test-driven-development`、`subagent-driven-development`；勾 `tasks.md` |
| 6 | 评审 | `/review`、`/qa`、`/cso`；`requesting-code-review` |
| 7 | 交付 | `openspec archive`；`/ship`、`/document-release`、`/retro`；`finishing-a-development-branch` |

OpenClaw 派发：Simple / Medium（gstack-lite）/ Heavy / Full / Plan — 见 gstack `docs/OPENCLAW.md`。

**硬规则**：动 `openclaw.json` / 多 agent / 协议 → 必须先 **OpenSpec change**。

## 输出（四行）

**阶段**（1～7）→ **缺口**（≤3）→ **下一步（唯一）** → 涉运行时/协议则 **先 OpenSpec change**。用户指令优先；勿谎称已跑 validate/doctor。

## References

`references/onboarding.md` · `references/glossary.md` · `references/install.md` · `references/pressure-prompts.md` · `references/examples.md` · `references/CHANGELOG-skill.md`。深入 OpenSpec 工作流时 **按 skill 名** 加载（勿写 `../` 路径）：`openspec-explore`、`openspec-propose`、`openspec-apply-change`、`openspec-archive-change`（彼处 description **勿**链 3devkit）。忌：三套说明书化；slash 须注明在已装 gstack 的 Agent 内。

# 新手指南：怎样真正用起来

本仓库的 GitHub 地址：https://github.com/mvgh2mv9ct-coder/studious-telegram

## 1. 你现在已经有什么？

- 13 个项目级 Skill 定义，位于 `.agents/skills/`。
- `AGENTS.md`，向支持它的 AI 解释怎样使用这些文件。
- GhostTrack 的上游 Git 子模块指针（未自动安装、未运行）。

## 2. 在电脑上的 Codex 使用

1. 在 Codex 中打开这份仓库的项目目录。若尚未下载到电脑，可通过 GitHub Desktop 克隆，或在安装 Git 的电脑中执行 `git clone https://github.com/mvgh2mv9ct-coder/studious-telegram.git`。
2. 让 Codex 读取项目的 `AGENTS.md`，再读取想用的技能说明。
3. 试试下面的指令：

   - `请读取 .agents/skills/grill-me/SKILL.md 和 .agents/skills/grilling/SKILL.md，按其中的流程帮我把“表格审核工具”的需求整理清楚。先问一个问题。`
   - `请使用 tdd 的方法，为表格审核程序设计测试；先让我确认测试边界。`
   - `请阅读 handoff 技能，整理今天的工作进度，方便下次继续。`

4. 若 Codex 原生支持从项目级目录发现 Skills，可按其支持的方式选择；若找不到，直接让其读取文件仍可使用说明内容。并非所有上游内建工具名都兼容 Codex。

## 3. GhostTrack

这个仓库保存一个上游 Git submodule 指针。如果你明确决定下载它，再了解 `git submodule update --init --recursive` 的作用：这会从上游取回源码，但**不会**自动安装依赖或运行其 Python 脚本。先检查作者、源代码、许可与依赖，且仅对自己的或获得明确授权的数据进行研究。

## 4. 何时选哪个

- **需求没想清楚**：`grill-me`
- **需要记录技术决定**：`grill-with-docs`
- **需要先写测试再开发**：`tdd`
- **需要浏览器自动化**：`agent-browser`（另装 CLI）
- **代码越来越乱**：`improve-codebase-architecture`
- **需要交给其他 AI 继续**：`handoff`
- **开始整理 GitHub Issue**：`setup-matt-pocock-skills` 后再用 `triage`

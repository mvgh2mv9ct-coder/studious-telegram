# AI Skills 工具仓库（Codex 优先）

> 一个供个人学习、AI 编程协作和开源工具研究使用的仓库。整理于 2026-10-23。

## 这里有什么？

- **10 个 AI Skills**：来自实际 GitHub 原项目，放在 `.agents/skills/<技能名>/`。Codex 打开本仓库时可发现这些项目级 Skills（具体使用取决于 Codex 版本及运行环境）。
- **GhostTrack**：记录官方上游地址与使用边界，**不自动运行、不复制其全部源码**。见 [GhostTrack 说明](tools/ghosttrack/README.md)。
- **原始来源与许可证**：见 [来源表](docs/UPSTREAM.md)。

## AI Skills 清单

| Skill | 一句话用途 |
| --- | --- |
| `find-skills` | 查找适合需求的 Agent Skills |
| `grill-me` | 持续提问，澄清需求与设计 |
| `grill-with-docs` | 澄清需求并更新项目术语和架构决策文档 |
| `improve-codebase-architecture` | 检查项目架构与改进方向 |
| `agent-browser` | 协助 AI 利用浏览器自动化 CLI（需要另装 CLI） |
| `tdd` | 测试驱动开发 |
| `setup-matt-pocock-skills` | 初始化 Matt Pocock 系列 Skills 的项目约定 |
| `frontend-design` | 指导更有辨识度的网页前端设计 |
| `handoff` | 在 AI 会话/工具之间交接任务进度 |
| `triage` | 分类与处理 GitHub Issues 等工作项目 |

## 怎么用（适合初学者）

1. 在电脑上通过 Codex **打开这个 GitHub 仓库**，或先克隆到本地再进入项目目录。
2. 查看 `.agents/skills/` 是否有以上 10 个技能文件夹。
3. 在 Codex 对话中先让 AI 阅读对应 `SKILL.md`，例如：「请使用 grill-me 帮我问清楚这个项目需求。」
4. 需要浏览器自动化时再单独安装 `agent-browser` CLI；只放入 Skill 定义不等于安装了浏览器运行程序。
5. 需要 Matt Pocock 系列的 Issue / 文档工作流时，先运行 `setup-matt-pocock-skills`；它可能修改仓库文件与标签，请先审核提议。

**重要区别**：Skills 是 AI 的工作指令，不等于手机 App、已经运行的软件，也不等于你在 ChatGPT 中可以直接调用一切本地程序。本仓库的 Skills 只是**项目级文件**，并未修改你的电脑或 ChatGPT 账号。

## 安全与更新

- 在运行任何第三方命令、脚本或联网操作之前，先审查原始来源、依赖和权限。
- 不要把手机号查询结果、他人隐私、账号密钥或班级个人资料提交到公开仓库。
- 仓库目前是 **Public（公开）**，任何人都可查看里面的内容。
- 上游内容会更新；本仓库内的 Skill 文件是录入时的快照，不会自动与上游同步。

请遵守各 Skill 随附的许可证与原作者声明；本仓库只是学习与组织入口，并不宣称拥有第三方项目的作者身份。

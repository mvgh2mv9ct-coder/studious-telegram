# AI Skills 工具仓库（Codex 优先）

收录截图里的 **10 个 AI Skills**、为其提供支持的 **3 个配套 Skills**，以及 **GhostTrack 原项目的 Git 子模块入口**。整理于 2026-10-23。

## 截图中的十个 Skill

| 技能 | 一句话用途 |
| --- | --- |
| `find-skills` | 发现其他可安装的 Agent Skills |
| `grill-me` | 通过连续追问把项目需求说清楚 |
| `grill-with-docs` | 追问并整理术语、架构决策文档 |
| `improve-codebase-architecture` | 检查并改进代码架构 |
| `agent-browser` | 协助运行浏览器自动化 CLI（需另外安装软件） |
| `tdd` | 测试驱动开发 |
| `setup-matt-pocock-skills` | 初始化 Matt Pocock 系列技能的项目配置 |
| `frontend-design` | 前端视觉与设计指导 |
| `handoff` | 为 AI 跨会话交接保存进度 |
| `triage` | 分类处理 GitHub Issues / PR |

额外包含依赖技能：`grilling`、`domain-modeling`、`codebase-design`。其中部分入口 Skill 很短，仅调用这些配套技能，所以必须一起保存。

## 使用导航

- [技能文件：.agents/skills/](.agents/skills/) — 13 个技能文件夹，附上必要的参考文档
- [新手使用手册：docs/START_HERE.md](docs/START_HERE.md)
- [真实上游来源与许可证：docs/UPSTREAM.md](docs/UPSTREAM.md)
- [安全规范：docs/SECURITY.md](docs/SECURITY.md)
- [GhostTrack 说明：tools/ghosttrack/README.md](tools/ghosttrack/README.md)
- [给 Codex 的仓库指令：AGENTS.md](AGENTS.md)

## 最快的使用办法

在 **Codex 中打开本仓库对应的本地项目目录**，然后输入：

> 请读取 `.agents/skills/grill-me/SKILL.md`，必要时继续读取 `.agents/skills/grilling/SKILL.md`，帮我一步一步澄清需求。

**注意：保存到 GitHub ≠ 已安装到你电脑或 ChatGPT 里。** GitHub 存的是文件，Codex 能否自动识别技能取决于版本及工作目录。你也可以让 AI 直接读取 `SKILL.md`。 `agent-browser` 的 CLI 和浏览器尚未安装。

GhostTrack 以链接到上游指定提交的 **Git submodule（子模块）** 形式挂接，主仓库没有复制它的源码。克隆子模块前应核查上游的依赖和许可证，且不得用它追踪或骚扰他人。

**本仓库为 Public（公开）**。勿上传个人手机号、令牌、账号密码、第三人的私密资料或班级个人信息。
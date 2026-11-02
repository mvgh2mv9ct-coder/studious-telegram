# AI extensions — curated upstream sources (2026-11-02)

These are **pinned Git submodules**, not installed or activated software. A gitlink records an upstream commit; source code is fetched only if you explicitly initialize that submodule. No third-party executable, model, 57GB dataset or API key is bundled.

| Module | Upstream | Pinned commit | Status / intent |
|---|---|---|---|
| `tools/ai-extensions/diagram-design` | [cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design) | `0cf73c3fcc56` | diagram generation; validate Chinese fonts and exported formats |
| `tools/ai-extensions/windows-mcp` | [CursorTouch/Windows-MCP](https://github.com/CursorTouch/Windows-MCP) | `c14240d42efc` | desktop automation; permissions and local access require review |
| `tools/ai-extensions/openmontage` | [calesthio/OpenMontage](https://github.com/calesthio/OpenMontage) | `195eab24478d` | video pipeline; check dependencies, model costs and GPU fit |
| `tools/ai-extensions/claude-mem` | [thedotmack/claude-mem](https://github.com/thedotmack/claude-mem) | `c239a048a8a0` | optional session memory; privacy and retention audit before enabling |
| `tools/ai-extensions/knowledge-work-plugins` | [anthropics/knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins) | `2574e29377c7` | job-specific workflow references; not auto-enabled |
| `tools/ai-extensions/free-claude-code` | [Alishahryar1/free-claude-code](https://github.com/Alishahryar1/free-claude-code) | `653a3444d43c` | optional alternate model routing; free providers have separate quotas |

Already bundled: the 13 existing AI Skills under `.agents/skills/`, including Matt Pocock skills. Do **not** overwrite or clone duplicate copies before examining the current local skill set.

## Planned trial order

1. Use existing `tdd`, `grill-me` (only on genuinely ambiguous tasks), `handoff` and `AGENTS.md` to verify a small spreadsheet/code change. Treat minimal reporting as a workflow policy, not a guarantee of token savings.
2. Initialize and audit `diagram-design` to generate one small chart; review its Chinese text and exports.
3. In a local, authorized test environment only, audit `windows-mcp` and allow only the desktop operations required for the task. Avoid unattended file deletion, network changes and administrator rights.
4. Evaluate `openmontage` with existing media, 30–60 seconds long, before choosing paid APIs or local generation models.
5. Keep `claude-mem`, `knowledge-work-plugins` and `free-claude-code` off by default. Evaluate separately only after checking data flows, pricing and runtime compatibility.

## Get source selectively

```powershell
git clone https://github.com/mvgh2mv9ct-coder/studious-telegram.git
cd studious-telegram
git submodule update --init -- tools/ai-extensions/diagram-design
```

To list pinned submodule versions without running their code: `git submodule status`. To get another module, replace the module path in the command. Do not use `--recursive` or initialize all modules by default. Avoid one-click installer scripts until reviewed.

## Deferred items (not installed, not submodules)

- `lyogavin/airllm`: heavily constrained GPU and memory bandwidth; run only if model profiling justifies it.
- `morluto/rea`: reverse engineering; only with appropriate authorization and a concrete need.
- `earthtojake/text-to-cad`: outside current needs; upstream match is tentative from the screenshot.
- `Renhuai123/ziwei-doushu`: separate cultural/software-research topic; dataset size is not accuracy evidence.
- `OpenSRE`: screenshot does not uniquely identify the intended upstream project.

All upstream licenses and usage conditions remain applicable. Review `docs/SECURITY.md` before initialization, especially because this host repository is public.

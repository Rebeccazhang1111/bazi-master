# bazi-master · 八字测算大师

一个专业的八字命盘分析 Agent Skill，支持专业版（~5000字）与通俗详解版（~20000字）两种报告输出。

遵循 [Agent Skills](https://agentskills.io) 开放规范（SKILL.md），兼容 Claude Code、Cursor、Codex、Kimi 等 40+ 支持 Skill 的 Agent。

## 目录结构

```
bazi-master/
├── SKILL.md                            # 技能入口（frontmatter + 分析流程 + 维度清单）
└── modules/
    ├── calculation.md                  # 日元能量计算、旺衰判断、喜用神
    ├── patterns.md                     # 格局判断、特殊格局
    ├── treasury.md                     # 四墓库、财富层级
    ├── advanced.md                     # 合化、长生、调候、太岁、空亡、象法
    ├── output-template.md              # 专业版报告模板
    └── output-template-detailed.md     # 通俗详解版报告模板（默认）
```

## 安装

### 方式一：一行命令安装（推荐）

```bash
npx skills add Rebeccazhang1111/bazi-master
```

[skills.sh](https://skills.sh) CLI 会自动识别你使用的 Agent（Claude Code / Cursor / Codex / Copilot 等 70+），并把 skill 放入对应的技能目录。需要本机装有 Node.js。

### 方式二：让 Agent 自己安装

直接对你的 Agent 说：

> 请从 GitHub 安装这个 skill：https://github.com/Rebeccazhang1111/bazi-master

支持联网的 Agent 通常会自动下载并放入正确的技能目录。

### 方式三：手动安装

```bash
git clone https://github.com/Rebeccazhang1111/bazi-master.git ~/.agents/skills/bazi-master
```

不同 Agent 的技能目录：
| Agent | 目录 |
|-------|------|
| Claude Code | `~/.claude/skills/` |
| Kimi / Codex 等（通用） | `~/.agents/skills/` 或项目内 `.agents/skills/` |

也可以在 Releases 页面下载 `bazi-master-skill.zip`，解压后手动放入上述目录。

## 使用

安装完成后无需重启，新开对话时 Agent 会自动识别。直接向 Agent 提供出生年月日时（注明农历/公历、性别），并请求八字分析即可。

## 声明

命理内容仅供娱乐与参考，不构成任何决策依据。请理性看待。

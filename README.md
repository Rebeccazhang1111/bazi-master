# bazi-master · 八字测算大师

一个专业的八字命盘分析 Agent Skill，支持专业版（~5000字）与通俗详解版（~20000字）两种报告输出。

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

本技能遵循 [Agent Skills](https://agentskills.io) 开放规范，兼容 Kimi、Claude 等支持 Skill 的 Agent。

**方式一：克隆到技能目录**

```bash
# 以 Kimi 为例，技能目录通常为 ~/.agents/skills/
git clone https://github.com/<你的用户名>/bazi-master.git ~/.agents/skills/bazi-master
```

**方式二：手动安装**

下载本仓库 ZIP 并解压，将 `bazi-master/` 文件夹放入你 Agent 的技能目录（如 `.agents/skills/`）即可。

## 使用

直接向你的 Agent 提供出生年月日时（注明农历/公历、性别），并请求八字分析，Agent 会自动加载本技能。

## 声明

命理内容仅供娱乐与参考，不构成任何决策依据。请理性看待。

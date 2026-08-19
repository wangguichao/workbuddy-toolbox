# Workbuddy 工具箱（workbuddy-toolbox）

> 一份「用 AI 助手自动化生活与工作」的 **100 条能力清单**，以及逐条扩展的 **可执行提示词 + 操作步骤**。

[![GitHub](https://img.shields.io/badge/GitHub-wangguichao%2Fworkbuddy--toolbox-181717?logo=github&logoColor=white)](https://github.com/wangguichao/workbuddy-toolbox)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![GitHub Stars](https://img.shields.io/github/stars/wangguichao/workbuddy-toolbox?style=social)](https://github.com/wangguichao/workbuddy-toolbox)
[![GitHub Forks](https://img.shields.io/github/forks/wangguichao/workbuddy-toolbox?style=social)](https://github.com/wangguichao/workbuddy-toolbox)
[![GitHub Issues](https://img.shields.io/github/issues/wangguichao/workbuddy-toolbox)](https://github.com/wangguichao/workbuddy-toolbox/issues)

## 这是什么

本项目整理了一份覆盖生活、工作、学习、娱乐等场景的 **100 条自动化能力清单**，并按照使用场景归纳为 **14 大主题模块**；每条能力再扩展出 **15~20 条** 可直接参考的内容，包含：

- **细分能力点**（5 条）：把一条能力拆成更小的可执行子任务
- **可执行提示词**（5 条）：可直接发送给 Workbuddy 的指令，已含具体参数与路径
- **操作步骤**（5~10 步）：对话式执行流程，展示你从向 Workbuddy 发指令到任务完成的完整交互

> 面向对象：使用 Workbuddy / Claude 桌面应用等 AI 助手，希望用自动化解放重复劳动的个人用户与开发者。

## 项目特性

- **100 条能力全覆盖**，14 大主题分类清晰，编号可追溯
- **1712 个扩展条目**，每条能力均有细分点、提示词、操作步骤
- **对话式执行**：只需向 Workbuddy 发送指令即可完成任务，无需自行搭建环境
- **零依赖**：纯 Markdown 文档，离线可读，易于维护和二次整理
- **MIT 开源**：自由使用、修改、商用

## 目录结构

```text
workbuddy-toolbox/
├── README.md               # 项目主页（本文件）
├── LICENSE                 # MIT 开源协议
├── CONTRIBUTING.md         # 贡献指南
├── docs/                   # 项目文档
│   ├── 分类总览.md          # 14 模块分类总览与编号索引
│   ├── 使用指南.md          # 如何挑选、落地与维护
│   └── 扩展模板.md          # 条目扩展规范（供贡献者参考）
├── 能力清单/
│   ├── 分类整理.md          # 100 条能力按 14 主题分类的清单
│   └── 能力扩展/            # 14 个模块的详细扩展
│       ├── README.md        # 扩展目录导航
│       ├── 模块01-系统安装与电脑维护.md
│       ├── 模块02-办公文档处理.md
│       ├── 模块03-表格与数据分析.md
│       ├── 模块04-图片处理.md
│       ├── 模块05-视频与音频处理.md
│       ├── 模块06-财务记账与报销.md
│       ├── 模块07-邮件与信息整理.md
│       ├── 模块08-教育学习与求职.md
│       ├── 模块09-内容创作与翻译.md
│       ├── 模块10-数据采集与资讯监控.md
│       ├── 模块11-办公自动化与效率.md
│       ├── 模块12-本地系统与生活工具.md
│       ├── 模块13-文件管理与安全备份.md
│       └── 模块14-开发与工程.md
├── skills/                 # 技能库：高频场景的 SKILL.md 技能文件
│   ├── README.md            # 技能库导航与模板说明
│   └── (财务/文档/表格等按模块组织的技能文件)
└── .github/                # GitHub 模板（PR / Issue）
    ├── PULL_REQUEST_TEMPLATE.md
    └── ISSUE_TEMPLATE/
```

## 技能库（Skills）

除能力清单外，项目还为高频场景准备了标准化的 **SKILL.md 技能文件**（试点 15 个），供 Workbuddy / Claude 加载使用：每个技能包含适用场景、可发送指令、处理要点、输出要求与注意事项。查看 [技能库导航](skills/README.md)。

### 从腾讯 SkillHub 安装技能

SkillHub 是腾讯的 AI 技能社区（[skillhub.cn/skills](https://skillhub.cn/skills)），**WorkBuddy 已集成 SkillHub CLI，可直接安装技能**，无需手动搜索。完整的 Top 50 技能清单见 [docs/SkillHub技能清单.md](docs/SkillHub技能清单.md)。

用法：直接对 WorkBuddy 说「帮我安装 SkillHub 上的『PDF 批处理大师』技能」，WorkBuddy 会自动安装；或执行 `skillhub install <技能名>`。

## 模块总览

| 模块 | 主题 | 原始条数 | 扩展条目 |
| --- | --- | --- | --- |
| 01 | [系统安装与电脑维护](能力清单/能力扩展/模块01-系统安装与电脑维护.md) | 8 | 140 |
| 02 | [办公文档处理](能力清单/能力扩展/模块02-办公文档处理.md) | 11 | 176 |
| 03 | [表格与数据分析](能力清单/能力扩展/模块03-表格与数据分析.md) | 7 | 116 |
| 04 | [图片处理](能力清单/能力扩展/模块04-图片处理.md) | 7 | 123 |
| 05 | [视频与音频处理](能力清单/能力扩展/模块05-视频与音频处理.md) | 11 | 185 |
| 06 | [财务记账与报销](能力清单/能力扩展/模块06-财务记账与报销.md) | 6 | 103 |
| 07 | [邮件与信息整理](能力清单/能力扩展/模块07-邮件与信息整理.md) | 6 | 100 |
| 08 | [教育学习与求职](能力清单/能力扩展/模块08-教育学习与求职.md) | 7 | 123 |
| 09 | [内容创作与翻译](能力清单/能力扩展/模块09-内容创作与翻译.md) | 7 | 115 |
| 10 | [数据采集与资讯监控](能力清单/能力扩展/模块10-数据采集与资讯监控.md) | 6 | 120 |
| 11 | [办公自动化与效率](能力清单/能力扩展/模块11-办公自动化与效率.md) | 4 | 65 |
| 12 | [本地系统与生活工具](能力清单/能力扩展/模块12-本地系统与生活工具.md) | 10 | 167 |
| 13 | [文件管理与安全备份](能力清单/能力扩展/模块13-文件管理与安全备份.md) | 7 | 121 |
| 14 | [开发与工程](能力清单/能力扩展/模块14-开发与工程.md) | 3 | 58 |
| | **合计** | **100** | **1712** |

## 快速开始

1. 在 [分类总览](docs/分类总览.md) 里找到你关心的一类事务，或直接浏览 [能力清单/分类整理.md](能力清单/分类整理.md)。
2. 打开对应模块文件，找到你想要的那条能力。
3. 使用方式：把「可执行提示词」复制给 Workbuddy，或按「操作步骤」中的对话流程与 Workbuddy 交互，由它自动完成整个任务（数据抓取、文件处理、定时调度等都由 Workbuddy 实现，无需自行搭建）。
4. 使用过程中发现缺步骤、写错、或有更好的方法，欢迎提交 Issue 或 PR。

## 如何贡献

我们欢迎任何形式的贡献，包括：补充新的能力条目、完善某一模块的操作步骤、修正错别字与链接、翻译文档等。请阅读 [CONTRIBUTING.md](CONTRIBUTING.md) 了解规范。

## 开源协议

本项目基于 [MIT 协议](LICENSE) 开源。你可以自由使用、修改、分发，甚至用于商业项目。

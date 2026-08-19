# Workbuddy 技能库（skills）

> 为高频自动化能力编写的标准化 **SKILL.md** 技能文件，供 Workbuddy / Claude 加载使用。每个技能文件都自包含：告诉 AI 何时触发、如何完成、输出什么。

试点阶段先覆盖 **15 个高频场景**，后续按模块逐步扩展。

## 使用方式

1. 把整个 `skills/` 目录或单个技能文件导入你的 AI 助手的技能目录（如 Claude 桌面应用可通过"保存技能"导入）。
2. 使用时直接说对应场景，AI 会自动匹配技能执行；或打开技能文件，把「向 Workbuddy 发送的指令」复制给它。

## 技能来源

本项目的技能标注来自三类来源：

- **Anthropic 官方技能**：Anthropic 维护的高质量技能（如 `docx` / `pdf` / `pptx` / `xlsx` / `schedule`），详见 [github.com/anthropics/skills](https://github.com/anthropics/skills)。
- **本项目自建技能**：`skills/` 目录下按模块组织的 SKILL.md，可直接复制使用。
- **腾讯 SkillHub**：面向中国用户的 AI 技能社区，收录大量精选技能，**WorkBuddy 可直接安装**。完整 Top 50 技能清单见 [docs/SkillHub技能清单.md](../docs/SkillHub技能清单.md)，可搜索下载：[skillhub.cn/skills](https://skillhub.cn/skills)。

> 各能力模块文件顶部均标注了「🔌 可用技能」，说明每条能力可直接引用的技能与获取方式，实现开箱即用。

## 技能清单

### 财务记账与报销

| 技能 | 对应能力 | 说明 |
| --- | --- | --- |
| [fund-daily-report](财务记账与报销/fund-daily-report.md) | #5 | 基金价格简报，定时邮件推送 |
| [invoice-ocr](财务记账与报销/invoice-ocr.md) | #14 | 发票识别，生成报销台账 |
| [bill-classifier](财务记账与报销/bill-classifier.md) | #18 | 支付宝/微信账单自动分类统计 |

### 办公文档处理

| 技能 | 对应能力 | 说明 |
| --- | --- | --- |
| [pdf-to-word](办公文档处理/pdf-to-word.md) | #3 | PDF 批量转 Word |
| [table-extract](办公文档处理/table-extract.md) | #27 | 批量提取文档表格汇总 Excel |
| [md-convert](办公文档处理/md-convert.md) | #57 | Markdown 转 Word/PDF/HTML |

### 表格与数据分析

| 技能 | 对应能力 | 说明 |
| --- | --- | --- |
| [excel-clean](表格与数据分析/excel-clean.md) | #7 | Excel 合并去重清洗画图 |
| [excel-format](表格与数据分析/excel-format.md) | #15 | 日期格式化与手机号脱敏 |
| [survey-analysis](表格与数据分析/survey-analysis.md) | #48 | 问卷数据汇总与图表 |

### 图片处理

| 技能 | 对应能力 | 说明 |
| --- | --- | --- |
| [image-ocr](图片处理/image-ocr.md) | #42 | 图片文字识别转 Word |

### 办公自动化与效率

| 技能 | 对应能力 | 说明 |
| --- | --- | --- |
| [daily-report](办公自动化与效率/daily-report.md) | #24 | 每日工作日报 |
| [meeting-notes](办公自动化与效率/meeting-notes.md) | #65 | 会议纪要提炼 |

### 文件管理与安全备份

| 技能 | 对应能力 | 说明 |
| --- | --- | --- |
| [batch-rename](文件管理与安全备份/batch-rename.md) | #21 | 批量重命名 |
| [desktop-organizer](文件管理与安全备份/desktop-organizer.md) | #62 | 桌面文件整理 |
| [backup](文件管理与安全备份/backup.md) | #80 | 定时备份 |

## 技能文件模板

每个 SKILL.md 遵循统一结构，frontmatter 的 `name` 与文件名一致，`description` 一句话描述触发场景：

```markdown
---
name: 技能名
description: 一句话触发描述（何时使用、含关键词）
---

# 技能名

## 适用场景
## 向 Workbuddy 发送的指令
## 处理要点
## 输出要求
## 注意事项
```

## 持续扩展

试点覆盖 15 个高频场景后，将按模块逐步为更多能力补充技能文件。新增技能请遵循上述模板，并同步登记到本 README。

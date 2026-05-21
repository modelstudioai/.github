# Model Studio AI

<p align="center">
  <a href="https://bailian.console.aliyun.com"><img src="https://img.shields.io/badge/Platform-%E9%98%BF%E9%87%8C%E4%BA%91%E7%99%BE%E7%82%BC-blue" alt="阿里云百炼"></a>
  <a href="https://www.npmjs.com/package/bailian-cli"><img src="https://img.shields.io/npm/v/bailian-cli.svg" alt="npm version"></a>
  <a href="./LICENSE"><img src="https://img.shields.io/badge/License-Apache%202.0-green.svg" alt="License"></a>
</p>

Model Studio AI 是[阿里云百炼（modelstudio](https://bailian.console.aliyun.com/cli?source_channel=cli_github&)）开源生态的技术阵地，期待和百万开发者一起，让 Agent 能力（生成图片、解析文档、调用工具、调度多模型）成为可复用的组件，通过自然语言描述需求即可串联成 Workflow。
为企业和开发者提供 AI Agent 应用开发所需的工具链、Skills 市场和行业最佳实践。


---

## 快速开始

### 安装阿里云百炼 CLI

```bash
npm install -g bailian-cli
```

> 前置要求：Node.js 18+

### 配置认证

前往 [阿里云百炼控制台](https://bailian.console.aliyun.com/cli?source_channel=key_github&) 获取 API Key，然后执行：

```bash
bl auth login --api-key YOUR_API_KEY
```

### 两种方式使用阿里云百炼能力

#### 方式一：在 AI 编程助手中对话调用（推荐）

阿里云百炼 CLI 安装后，会自动向你的 AI 编程助手注册 Skill。无需手动配置 API Key，直接用自然语言描述需求：

**在 Qwen Code 中**
```
> 请帮我全局安装阿里云百炼 CLI 命令行工具
✓ bailian-cli 安装完成
✓ 认证成功！已连接到阿里云百炼平台

> 根据这个 IP 形象，帮我设计一整套适用于电商售卖的产品方案图
✓ 已上传图片: ip-character.jpg
✓ 已生成 6 张电商产品方案图
```

**在 Claude Code 中**
```
> 把这份销售报表转成柱状图
✓ 已生成柱状图，保存为 sales_chart.png

> 给这个产品写一段小红书风格的种草文案
✓ 已生成 3 版文案，风格分别为活泼、专业、场景化
```

#### 方式二：在终端中直接调用

```bash
# 生成图片
bl image generate --prompt "白色无线蓝牙耳机电商主图"

# 编辑图片
bl image edit --image ./ip-character.jpg

# 列出可用能力
bl capabilities

# 搜索 Skills 市场
bl skill search "合同审查"

# 安装 Skill
bl skill install contract-review

# 运行 Workflow
bl workflow run "分析这份用户调研数据，提取 Top 5 痛点"
```

---
## 核心能力一览

阿里云百炼 CLI 支持 AI Agent 自动调度 10+ 大模型能力：

| 能力 | 自然语言调用示例 | 终端命令示例 | 适用场景 |
|------|-----------------|-------------|---------|
| **图像生成** | "生成一张科技风格的 Banner" | `bl image generate --prompt "..."` | 电商主图、营销物料、社交媒体 |
| **图像编辑** | "根据这个 IP 形象设计产品方案图" | `bl image edit --image ./...` | 产品方案、IP 延展、视觉设计 |
| **视频生成** | "把这张图做成 3 秒产品展示视频" | `bl video generate --image ./...` | 短视频、广告、产品演示 |
| **文档解析** | "提取合同里的付款条款" | `bl document parse ./contract.pdf` | 合同审查、报告摘要、知识归档 |
| **代码生成** | "写一个 Python 脚本批量处理 Excel" | `bl code generate "..."` | Vibe Coding、自动化脚本、数据处理 |
| **数据分析** | "分析这份销售数据，找出增长原因" | `bl data analyze ./sales.csv` | 经营分析、用户洞察、趋势预测 |
| **智能客服** | "给这位用户的售后问题生成回复" | `bl agent chat --context "..."` | 客服自动化、工单处理、用户运营 |
| **知识问答** | "基于我们公司产品手册回答这个问题" | `bl knowledge query "..."` | 企业知识库、产品咨询、技术支持 |

## 核心项目

激情创作中 ... ...


---

## 行业 Workflow 示例

### 电商内容生产

```
产品图片 → [图像生成/编辑] → 多场景商品图（白底/场景/细节）
         → [文案生成]       → 淘宝标题 / 小红书种草 / 直播话术
         → [视频生成]       → 15秒产品展示视频
         → [数据洞察]       → 竞品定价建议 + 卖点差异化分析
```

**Agent 对话调用**
```
> 为这款新上市的运动鞋生成全套营销素材：商品图、各平台文案、短视频，再分析一下竞品价格
```

**终端命令调用**
```bash
bl image generate --prompt "运动鞋电商主图，白色背景"
bl image generate --prompt "运动鞋场景图，户外跑道"
bl video generate --image ./shoes.jpg --duration 15
bl workflow run "分析运动鞋竞品价格并给出定价建议"
```

### 企业文档处理

```
合同/报告 → [文档解析]   → 结构化文本提取
          → [信息抽取]   → 关键条款、金额、日期、责任人
          → [风险标记]   → 自动标出高风险条款
          → [摘要生成]   → 管理层速览版本
          → [知识归档]   → 自动归入企业知识库
```

**Agent 对话调用**
```
> 审查这份采购合同，标出风险点，生成一份给法务总监的摘要
```

**终端命令调用**
```bash
bl document parse ./contract.pdf
bl workflow run "审查合同风险并生成法务摘要"
```

### 金融研报分析

```
研报/公告 → [文档解析]   → 全文结构化
          → [摘要提取]   → 核心观点与投资逻辑
          → [数据抽取]   → 财务指标、估值数据、风险因素
          → [标签生成]   → 行业/主题/sentiment 自动分类
          → [对比分析]   → 与历史报告或竞品报告对比
```

**Agent 对话调用**
```
> 分析这份 quarterly report，提取关键财务数据，生成投资者沟通摘要，标出风险因素
```

**终端命令调用**
```bash
bl document parse ./report.pdf
bl data analyze ./financials.csv
bl workflow run "分析财报并生成投资者摘要"
```

---

## 生态合作

阿里云百炼 CLI 与主流 AI 开发工具深度集成，一次安装，多处使用：

<p align="center">
  <a href="https://github.com/modelcontextprotocol">MCP</a> ·
  <a href="https://github.com/mannaandpoem/OpenManus">OpenManus</a> ·
  <a href="https://github.com/browser-use/browser-use">Browser Use</a> ·
  <a href="https://github.com/open-webui/open-webui">Open WebUI</a>
</p>

无论你用 Claude Code、Qwen Code、Cursor、Qoder 还是 Windsurf，阿里云百炼 CLI 安装后自动注册为 Agent Skill，零配置即可调用。

---

## 为什么选择阿里云百炼 CLI？

| 特性 | 说明 |
|------|------|
| **自然语言驱动** | 不需要记命令，跟你的 AI 编程助手说需求即可 |
| **自动注册 Skill** | 安装后自动集成 Claude Code / Qwen Code，无需手动配置 API Key |
| **双模式调用** | 既支持 Agent 对话调用，也支持终端命令行直接操作 |
| **能力即插即用** | 图像、视频、文档、代码等能力统一入口，按需调度 10+ 模型 |
| **Vibe Coding 原生** | 专为 AI 编程助手设计，支持迭代式开发、实时调试 |
| **MCP 兼容** | 符合 Model Context Protocol 标准，可接入任意 MCP 客户端 |
| **Skills 市场** | 支持搜索、安装、更新、发布 Skills，生态持续扩展 |
| **中文场景优化** | 从文档解析到文案生成，深度适配中文业务场景 |
| **阿里云背书** | 通义大模型 + 阿里云百炼平台，企业级安全与稳定性 |

---

## 加入社区

欢迎提交issue交流！
社区、博客、交流群建设中

---

## 贡献指南

激情建设中 ... ...

---

<p align="center">
  <sub>Built with ❤️ by the Model Studio AI team, powered by <a href="https://bailian.console.aliyun.com/cli?source_channel=cli_github&">阿里云百炼</a></sub>
</p>

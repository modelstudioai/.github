<p align="center">
  <strong>Model Studio AI</strong>
</p>

<p align="center">
  <a href="https://bailian.console.aliyun.com/cli?source_channel=cli_github&"><img src="https://img.shields.io/badge/ModelStudio-blue?logo=alibabacloud" alt="ModelStudio"></a>
  <a href="https://www.npmjs.com/package/bailian-cli"><img src="https://img.shields.io/npm/v/bailian-cli.svg?logo=npm" alt="npm"></a>
  <a href="https://github.com/modelstudioai/skills"><img src="https://img.shields.io/github/stars/modelstudioai/skills?style=social" alt="Stars"></a>
  <a href="https://github.com/modelstudioai/.github/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-Apache%202.0-green.svg" alt="License"></a>
</p>

<p align="center">
  <a href="#english">English</a> · <a href="#中文">中文</a>
</p>

---

## English

### About

Model Studio AI is the open-source home of [ModelStudio](https://bailian.console.aliyun.com/cli?source_channel=cli_github&). We publish tools, verified skills, and reference implementations that help developers build with large models — from image and video generation to document understanding and multi-model orchestration.

### Repositories

| Repository | Description |
|:-----------|:------------|
| **[skills](https://github.com/modelstudioai/skills)** | 26 curated & verified skills across 6 categories. Works with Claude Code, Qwen Code, and any MCP-compatible client. |
| **[awesome-happyhorse-prompts](https://github.com/modelstudioai/awesome-happyhorse-prompts)** | Prompts, API patterns, and creative workflows for HappyHorse video generation models. |
| **[LiveTranslate-Demo](https://github.com/modelstudioai/LiveTranslate-Demo)** | Real-time multilingual translation demo powered by ModelStudio streaming APIs. |

### Quick Start

```bash
# Install the ModelStudio CLI (Node.js 18+)
npm install -g bailian-cli

# Authenticate (get your key at https://bailian.console.aliyun.com/cli?source_channel=key_github)
bl auth login --api-key YOUR_API_KEY
```

Once installed, the CLI auto-registers as a skill in **Claude Code**, **Qwen Code**, **Cursor**, and any MCP-compatible client — zero extra config. Use natural language to invoke capabilities:

```
> Generate a product showcase image with white background
> Parse this contract and highlight payment terms
> Create a 3-second video from this image
```

### Core Capabilities

| Capability | Example | Use Cases |
|:-----------|:--------|:----------|
| Image Generation | "Generate a tech-style banner" | E-commerce, marketing, social media |
| Image Editing | "Design product mockups from this IP character" | Product design, visual branding |
| Video Generation | "Turn this image into a 3s product demo" | Short-form video, ads |
| Document Parsing | "Extract payment terms from this contract" | Contract review, knowledge archiving |
| Code Generation | "Write a Python script to batch-process Excel files" | Automation, data processing |
| Data Analysis | "Analyze this sales data and identify growth drivers" | Business analytics, trend forecasting |

### Ecosystem

Our projects integrate with the broader AI development ecosystem:

<p align="center">
  <a href="https://modelcontextprotocol.io">MCP</a> · 
  <a href="https://github.com/anthropics/claude-code">Claude Code</a> · 
  <a href="https://github.com/QwenLM/qwen-code">Qwen Code</a> · 
  <a href="https://github.com/mannaandpoem/OpenManus">OpenManus</a> · 
  <a href="https://github.com/browser-use/browser-use">Browser Use</a> · 
  <a href="https://github.com/open-webui/open-webui">Open WebUI</a>
</p>

## 中文

### 关于

Model Studio AI 是[阿里云百炼](https://bailian.console.aliyun.com/cli?source_channel=cli_github&)的开源技术阵地。我们发布工具、经验证的 Skills 和参考实现，帮助开发者基于大模型构建应用——从图像和视频生成，到文档理解和多模型调度。

### 核心项目

| 仓库 | 简介 |
|:-----|:-----|
| **[skills](https://github.com/modelstudioai/skills)** | 26 个经验证的 Skills，覆盖 6 大场景。支持 Claude Code、Qwen Code 和任意 MCP 客户端。 |
| **[awesome-happyhorse-prompts](https://github.com/modelstudioai/awesome-happyhorse-prompts)** | 精选 HappyHorse 视频生成模型的 prompt、API 调用模式与创意工作流。 |
| **[LiveTranslate-Demo](https://github.com/modelstudioai/LiveTranslate-Demo)** | 基于阿里云百炼流式 API 的实时多语言翻译 Demo。 |

### 快速开始

```bash
# 安装阿里云百炼 CLI（需要 Node.js 18+）
npm install -g bailian-cli

# 配置 API Key（前往 https://bailian.console.aliyun.com/cli?source_channel=key_github 获取）
bl auth login --api-key YOUR_API_KEY
```

安装后，阿里云百炼 CLI 会自动向 Claude Code / Qwen Code / Cursor 等 AI 编程助手注册 Skill，**无需手动配置**，直接用自然语言描述需求即可：

> 帮我生成一张科技风格的 Banner，蓝色渐变背景

> 把这份合同解析出来，标出付款条款和风险点

> 把这张图做成 3 秒的产品展示视频

### 核心能力

| 能力 | 自然语言调用示例 | 适用场景 |
|:-----|:----------------|:---------|
| 图像生成 | "生成一张电商主图，白色背景" | 电商、营销、社交媒体 |
| 图像编辑 | "根据这个 IP 形象设计产品方案图" | 产品设计、IP 延展 |
| 视频生成 | "把这张图做成 3 秒展示视频" | 短视频、广告 |
| 文档解析 | "提取合同里的付款条款" | 合同审查、知识归档 |
| 代码生成 | "写个 Python 脚本批量处理 Excel" | 自动化、数据处理 |
| 数据分析 | "分析这份销售数据的增长原因" | 经营分析、趋势洞察 |

### 行业 Workflow 示例

**电商内容生产**
```
产品图片 → [图像生成/编辑] → 多场景商品图
         → [文案生成]       → 淘宝标题 / 小红书种草 / 直播话术
         → [视频生成]       → 15 秒产品展示视频
         → [数据洞察]       → 竞品定价 + 卖点差异化
```

**企业文档处理**
```
合同/报告 → [文档解析] → 结构化提取 → [风险标记] → [摘要生成] → 管理层速览
```

### 生态合作

阿里云百炼 CLI 与主流 AI 开发工具深度集成，一次安装，多处使用：

<p align="center">
  <a href="https://modelcontextprotocol.io">MCP</a> · 
  <a href="https://github.com/anthropics/claude-code">Claude Code</a> · 
  <a href="https://github.com/QwenLM/qwen-code">Qwen Code</a> · 
  <a href="https://github.com/mannaandpoem/OpenManus">OpenManus</a> · 
  <a href="https://github.com/browser-use/browser-use">Browser Use</a> · 
  <a href="https://github.com/open-webui/open-webui">Open WebUI</a>
</p>

### 社区

- **钉钉开发者群**：扫码加入，获取最新动态与技术支持
  <p align="center">
  欢迎加入钉钉群交流
</p>
<p align="center">
<img width="200" height="200" alt="qr_with_avatar" src="https://github.com/user-attachments/assets/57a43cb4-c9cb-4591-8cec-959cd6e2cd09" />
</p>

<!-- Replace with actual QR code image -->
<!-- <img src="https://raw.githubusercontent.com/modelstudioai/.github/main/assets/dingtalk-qr.png" width="200"> -->

---


<p align="center">
  <sub> Built with ❤️ by the Model Studio </a></sub>
</p>

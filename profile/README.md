<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://img.alicdn.com/imgextra/i1/O1CN01CEGjGx1GZ3E3bJMHS_!!6000000000635-2-tps-2000-400.png">
    <source media="(prefers-color-scheme: light)" srcset="https://img.alicdn.com/imgextra/i1/O1CN01CEGjGx1GZ3E3bJMHS_!!6000000000635-2-tps-2000-400.png">
    <img alt="Model Studio AI" src="https://img.alicdn.com/imgextra/i1/O1CN01CEGjGx1GZ3E3bJMHS_!!6000000000635-2-tps-2000-400.png" width="600">
  </picture>
</p>

<p align="center">
  <strong>The open-source home of <a href="https://bailian.console.aliyun.com">Alibaba Cloud Model Studio</a></strong><br>
  Tools, skills, and reference implementations for building with large models.
</p>

<p align="center">
  <a href="https://bailian.console.aliyun.com/cli"><img src="https://img.shields.io/badge/ModelStudio-blue?logo=alibabacloud" alt="ModelStudio"></a>
  <a href="https://www.npmjs.com/package/bailian-cli"><img src="https://img.shields.io/npm/v/bailian-cli.svg?logo=npm" alt="npm"></a>
  <a href="https://github.com/modelstudioai/skills"><img src="https://img.shields.io/github/stars/modelstudioai/skills?style=social" alt="Stars"></a>
  <a href="https://github.com/modelstudioai/.github/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-Apache%202.0-green.svg" alt="License"></a>
</p>

<p align="center">
  <a href="https://modelcontextprotocol.io">MCP</a> ·
  <a href="https://github.com/anthropics/claude-code">Claude Code</a> ·
  <a href="https://github.com/QwenLM/qwen-code">Qwen Code</a> ·
  <a href="https://github.com/mannaandpoem/OpenManus">OpenManus</a> ·
  <a href="https://github.com/browser-use/browser-use">Browser Use</a> ·
  <a href="https://github.com/open-webui/open-webui">Open WebUI</a>
</p>

---

## Quick Start

```bash
# Install the CLI (Node.js 18+)
npm install -g bailian-cli

# Authenticate — get your key at https://bailian.console.aliyun.com
bl auth login --api-key YOUR_API_KEY
```

The CLI auto-registers as a skill in **Claude Code**, **Qwen Code**, **Cursor**, and any MCP-compatible client. No extra config needed.

```
> Generate a product showcase image with white background
> Parse this contract and highlight payment terms
> Create a 3-second video from this image
```

## Repositories

| Repository | Description |
|:-----------|:------------|
| **[skills](https://github.com/modelstudioai/skills)** | 26 curated & verified skills across 6 categories. Works with Claude Code, Qwen Code, and any MCP client. |
| **[awesome-happyhorse-prompts](https://github.com/modelstudioai/awesome-happyhorse-prompts)** | Prompts, API patterns, and creative workflows for HappyHorse video generation models. |
| **[LiveTranslate-Demo](https://github.com/modelstudioai/LiveTranslate-Demo)** | Real-time multilingual translation demo powered by ModelStudio streaming APIs. |

## Capabilities

| Capability | Example | Use Cases |
|:-----------|:--------|:----------|
| Image Generation | "Generate a tech-style banner" | E-commerce, marketing |
| Image Editing | "Design product mockups from this IP character" | Product design |
| Video Generation | "Turn this image into a 3s product demo" | Short-form video, ads |
| Document Parsing | "Extract payment terms from this contract" | Contract review |
| Code Generation | "Write a Python script to batch-process Excel" | Automation |
| Data Analysis | "Analyze this sales data and identify growth drivers" | Business analytics |

<details>
<summary><strong>中文</strong></summary>

### 关于

Model Studio AI 是[阿里云百炼](https://bailian.console.aliyun.com)的开源技术阵地。我们发布工具、经验证的 Skills 和参考实现，帮助开发者基于大模型构建应用。

### 快速开始

```bash
# 安装阿里云百炼 CLI（需要 Node.js 18+）
npm install -g bailian-cli

# 配置 API Key（前往 https://bailian.console.aliyun.com 获取）
bl auth login --api-key YOUR_API_KEY
```

安装后自动向 Claude Code / Qwen Code / Cursor 等 AI 编程助手注册 Skill，无需手动配置。

### 核心项目

| 仓库 | 简介 |
|:-----|:-----|
| **[skills](https://github.com/modelstudioai/skills)** | 26 个经验证的 Skills，覆盖 6 大场景。支持 Claude Code、Qwen Code 和任意 MCP 客户端。 |
| **[awesome-happyhorse-prompts](https://github.com/modelstudioai/awesome-happyhorse-prompts)** | 精选 HappyHorse 视频生成模型的 prompt、API 调用模式与创意工作流。 |
| **[LiveTranslate-Demo](https://github.com/modelstudioai/LiveTranslate-Demo)** | 基于阿里云百炼流式 API 的实时多语言翻译 Demo。 |

### 核心能力

| 能力 | 示例 | 场景 |
|:-----|:-----|:-----|
| 图像生成 | "生成一张电商主图，白色背景" | 电商、营销 |
| 图像编辑 | "根据这个 IP 形象设计产品方案图" | 产品设计 |
| 视频生成 | "把这张图做成 3 秒展示视频" | 短视频、广告 |
| 文档解析 | "提取合同里的付款条款" | 合同审查 |
| 代码生成 | "写个 Python 脚本批量处理 Excel" | 自动化 |
| 数据分析 | "分析这份销售数据的增长原因" | 经营分析 |

### 社区

欢迎加入钉钉群交流：

<p align="center">
<img width="200" height="200" alt="钉钉群二维码" src="https://github.com/user-attachments/assets/57a43cb4-c9cb-4591-8cec-959cd6e2cd09" />
</p>

</details>

## Contributing

We welcome contributions from developers worldwide.
- **Report issues** — Open an issue in the relevant repository
- **Submit PRs** — Follow the contributing guidelines in each repo

---

<p align="center">
  <sub>Built with ❤️ by the <a href="https://bailian.console.aliyun.com">Model Studio</a> team</sub>
</p>

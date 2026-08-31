
<p align="center">
  <strong>The open-source home of Model Studio</strong><br>
  Tools, skills, and reference implementations for building with large models.
</p>

<p align="center">
  <a href="https://bailian.console.aliyun.com/cli?source_channel=cli_github&"><img src="https://img.shields.io/badge/ModelStudio-blue?logo=alibabacloud" alt="ModelStudio"></a>
  <a href="https://www.npmjs.com/package/bailian-cli"><img src="https://img.shields.io/npm/v/bailian-cli.svg?logo=npm" alt="npm"></a>
  <a href="https://github.com/modelstudioai/skills"><img src="https://img.shields.io/github/stars/modelstudioai/skills?style=social" alt="Stars"></a>
  <a href="https://github.com/modelstudioai/.github/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-Apache%202.0-green.svg" alt="License"></a>
</p>

<p align="center">
  <a href="https://modelcontextprotocol.io">MCP</a> ·
  <a href="https://github.com/anthropics/claude-code">Claude Code</a> ·
  <a href="https://github.com/QwenLM/qwen-code">Qwen Code</a> ·
  <a href="https://www.cursor.com">Cursor</a> ·
  <a href="https://github.com/cline/cline">Cline</a> ·
  <a href="https://windsurf.com">Windsurf</a> ·
  <a href="https://github.com/browser-use/browser-use">Browser Use</a> ·
  <a href="https://github.com/open-webui/open-webui">Open WebUI</a>
</p>

<img width="1920" height="1080" alt="githuborg配图图" src="https://github.com/user-attachments/assets/14550956-034f-41d5-985b-b44876f06d5a" />

---

## English

### About

Model Studio AI is the open-source home of [ModelStudio](https://bailian.console.aliyun.com/cli?source_channel=cli_github&). We publish tools, verified skills, and reference implementations that help developers build with large models — from image and video generation to document understanding and multi-model orchestration.


### Quick Start

```bash
# Install the CLI (Node.js 18+)
npm install -g bailian-cli

# Authenticate — get your key at https://bailian.console.aliyun.com/cn-beijing/?source_channel=key_github&tab=app#/api-key
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
| **[cli](https://github.com/modelstudioai/cli)** | The official Model Studio CLI (`bl`) for AI Agent frameworks. Auto-registers as a skill in Claude Code, Qwen Code, Cursor, Cline, Windsurf, and any MCP-compatible client. |
| **[OpenAgentPack](https://github.com/modelstudioai/OpenAgentPack)** | The open-source IaC control plane for managed AI agents. Manage, review, and migrate agent assets with Git and YAML; preview changes through `validate → plan → apply`, and target multiple managed-agent platforms from one core declaration to reduce platform lock-in. |
| **[skills](https://github.com/modelstudioai/skills)** | The official Agent Skills collection — 26 curated community skills across 6 scenarios (skill management, code, design, docs, video, testing), plus first-party skills bundled from [`modelstudioai/cli`](https://github.com/modelstudioai/cli) and this repo. Works with Claude Code, Qwen Code, and any MCP client. |
| **[openwork](https://github.com/modelstudioai/openwork)** | Local-first desktop Agent for end-to-end AI workflows — open-source companion app to Model Studio. |
| **[awesome-happyhorse-prompts](https://github.com/modelstudioai/awesome-happyhorse-prompts)** | Prompts, storyboards, and verified creative workflows for the HappyHorse 1.0 / 1.1 video generation models. |
| **[livetranslatedemo](https://github.com/modelstudioai/livetranslatedemo)** | Real-time multilingual translation demo powered by ModelStudio streaming APIs. |
| **[modelstudioai.github.io](https://github.com/modelstudioai/modelstudioai.github.io)** | Source of the official site [modelstudioai.github.io](https://modelstudioai.github.io) — community Showcase, guides, playbook, FAQ, and video tutorials. |

> See all repositories → [github.com/orgs/modelstudioai/repositories](https://github.com/orgs/modelstudioai/repositories)

## Docs & Community

- **Docs / Showcase / Playbook** → [modelstudioai.github.io](https://modelstudioai.github.io) — guides, community case Showcase, capability playbook, FAQ, and video tutorials.
- **Join the Bailian Open-Source Developer Program** → [bailian.console.aliyun.com/opensource](http://bailian.console.aliyun.com/opensource) — get a certified badge, community perks, and priority collaboration opportunities.

## Capabilities

| Capability | Example | Use Cases |
|:-----------|:--------|:----------|
| Image Generation | "Generate a tech-style banner" | E-commerce, marketing |
| Image Editing | "Design product mockups from this IP character" | Product design |
| Video Generation | "Turn this image into a 3s product demo" | Short-form video, ads |
| Document Parsing | "Extract payment terms from this contract" | Contract review |
| Code Generation | "Write a Python script to batch-process Excel" | Automation |
| Data Analysis | "Analyze this sales data and identify growth drivers" | Business analytics |

## 中文

### 关于

Model Studio AI 是[阿里云百炼](https://bailian.console.aliyun.com/cli?source_channel=cli_github&)的开源主页。我们发布工具、经验证的 Skills 和参考实现，帮助开发者基于大模型构建应用——从图像和视频生成，到文档理解和多模型调度。


### 快速开始

```bash
# 安装阿里云百炼 CLI（需要 Node.js 18+）
npm install -g bailian-cli

# 配置 API Key（前往 https://bailian.console.aliyun.com/cn-beijing/?source_channel=key_github&tab=app#/api-key 获取）
bl auth login --api-key YOUR_API_KEY
```

安装后自动向 Claude Code / Qwen Code / Cursor 等 AI 编程助手注册 Skill，无需手动配置。

### 核心项目

| 仓库 | 简介 |
|:-----|:-----|
| **[cli](https://github.com/modelstudioai/cli)** | 阿里云百炼官方 CLI（`bl`），为 AI Agent 框架而生。安装后自动向 Claude Code / Qwen Code / Cursor / Cline / Windsurf 等 MCP 兼容客户端注册 Skill。 |
| **[OpenAgentPack](https://github.com/modelstudioai/OpenAgentPack)** | 面向托管 AI Agent 的开源 IaC 控制平面。用 Git 和 YAML 管理、审查并迁移 Agent 资产，通过 `validate → plan → apply` 预览和执行变更，以一份核心声明对接多个托管 Agent 平台，降低平台绑定。 |
| **[skills](https://github.com/modelstudioai/skills)** | 官方 Agent Skills 集合——26 个社区精选 Skills 覆盖 Skill 管理、代码开发、设计创意、文档、视频、测试 6 大场景，另含由 [`modelstudioai/cli`](https://github.com/modelstudioai/cli) 和本仓库提供的一方 Skills。支持 Claude Code、Qwen Code 和任意 MCP 客户端。 |
| **[openwork](https://github.com/modelstudioai/openwork)** | 本地优先的桌面 Agent，端到端跑通 AI 工作流的开源桌面应用。 |
| **[awesome-happyhorse-prompts](https://github.com/modelstudioai/awesome-happyhorse-prompts)** | 精选 HappyHorse 1.0 / 1.1 视频生成模型的 prompt、故事板与创意工作流。 |
| **[livetranslatedemo](https://github.com/modelstudioai/livetranslatedemo)** | 基于阿里云百炼流式 API 的实时多语言翻译 Demo。 |
| **[modelstudioai.github.io](https://github.com/modelstudioai/modelstudioai.github.io)** | 官网 [modelstudioai.github.io](https://modelstudioai.github.io) 源码——社区案例 Showcase、上手教程、Playbook、FAQ 与视频教程。 |

> 查看全部仓库 → [github.com/orgs/modelstudioai/repositories](https://github.com/orgs/modelstudioai/repositories)


### 文档与社区

- **文档 / 案例 Showcase / Playbook** → [modelstudioai.github.io](https://modelstudioai.github.io)——上手教程、社区案例 Showcase、能力 Playbook、FAQ 与视频教程。
- **加入百炼开源开发者计划** → [bailian.console.aliyun.com/opensource](http://bailian.console.aliyun.com/opensource)——开通认证开发者权益、社区礼品与优先合作机会。


### 生态合作

欢迎加入钉钉群交流：

<p align="center">
<img width="200" height="200" alt="钉钉群二维码" src="https://github.com/user-attachments/assets/57a43cb4-c9cb-4591-8cec-959cd6e2cd09" />
</p>

### 社区

We welcome contributions from developers worldwide.
- **Report issues** — Open an issue in the relevant repository
- **Submit PRs** — Follow the contributing guidelines in each repo

---

<p align="center">
  <sub>Built with ❤️ by the <a href="https://bailian.console.aliyun.com/cli?source_channel=cli_github&">Model Studio</a> team</sub>
</p>

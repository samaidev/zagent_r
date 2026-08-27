# ZAgent

轻量级跨平台 AI 智能体 —— 流式对话 · 工具调用 · 工作流自动化 · 隐身浏览器 · 持久化记忆

[![Download](https://img.shields.io/badge/%E4%B8%8B%E8%BD%BD-%E6%9C%80%E6%96%B0%E7%89%88-blue)](https://github.com/samaidev/zagent_r/releases/latest)
[![PyPI](https://img.shields.io/pypi/v/samai-zagent)](https://pypi.org/project/samai-zagent/)
[![Platform](https://img.shields.io/badge/platform-Linux%20%7C%20macOS%20%7C%20Windows%20%7C%20Android-green)](#-下载)

---

## 简介 / Overview

ZAgent 是一个轻量级、跨平台的自主 AI 智能体，原生支持 Linux / macOS / Windows / Android，连接 AICQ 消息平台提供实时 AI 助手服务。本仓是**公开发布仓**，只提供安装方法与成品下载；项目源码与开发请见内部仓库。

ZAgent is a lightweight cross-platform autonomous AI agent for Linux / macOS / Windows / Android. This is the **release-only repository**: binaries and install instructions live here, development happens internally.

## 主要功能 / Key Features

- **流式对话** — 实时 SSE 回复，可折叠推理面板，Markdown / 代码高亮渲染
- **内置工具调用** — 文件读写、命令执行、代码运行、网页搜索与阅读、浏览器自动化
- **子代理编排** — 主代理委托任务给子代理，完成后自动唤醒主代理继续
- **工作流自动化** — 可视化编辑器 + 调度器，支持定时 / 事件触发多步骤任务
- **隐身浏览器** — 反检测 Chrome 自动化，可复用已登录站点配置
- **持久化记忆** — SQLite 关键词记忆检索，跨会话上下文延续
- **闹钟唤醒** — 任务延时等待，到点自动开会话继续推进
- **免费模型通道** — 内置 keyless 免费模型接入，开箱即用

## 安装 / Install

### 方式一：pip（推荐）

```bash
pip install samai-zagent
```

安装后运行：

```bash
zagent          # 默认 Web UI :8181，浏览器打开 http://localhost:8181
```

### 方式二：一键脚本

| 平台 | 命令 |
|------|------|
| Linux / macOS | `curl -fsSL https://zagent.samai.cc/install.sh \| bash` |
| Windows (PowerShell) | `irm https://zagent.samai.cc/install.ps1 \| iex` |

### 方式三：Android APK

1. 打开 [Releases 最新版](https://github.com/samaidev/zagent_r/releases/latest)
2. 下载 `zagent-android-arm64-*.apk`
3. 安装前允许「未知来源应用」；升级直接覆盖安装，数据自动保留

### 使用入门

首次启动后在 Web UI「设置」中配置 LLM 接口（支持任意 OpenAI 兼容 API，或直接选用内置免费模型），之后即可在聊天框下发任务：让 Agent 执行命令、生成文档（PPT / Word / Excel / PDF）、搭建网页并通过隧道分享等。

## 下载 / Download

**👉 [点击下载最新版](https://github.com/samaidev/zagent_r/releases/latest)**

| 平台 | 文件 |
|------|------|
| Linux x86_64 | `zagent-linux-amd64.tar.gz` |
| Linux ARM64 | `zagent-linux-arm64.tar.gz` |
| macOS Intel | `zagent-darwin-amd64.tar.gz` |
| macOS Apple Silicon | `zagent-darwin-arm64.tar.gz` |
| Windows x86_64 | `zagent-windows-amd64.zip` |
| Windows ARM64 | `zagent-windows-arm64.zip` |
| Android ARM64 | `zagent-android-arm64-*.apk` |

<!-- SAMAI-CI-RELEASES-START -->
<!-- 本区块由 CI 在发版时自动维护；完整版本列表见 Releases 页面 -->
<!-- SAMAI-CI-RELEASES-END -->

## 链接 / Links

- **官网 Website**: [zagent.samai.cc](https://zagent.samai.cc)
- **在线体验 Demo**: [zagent.aitun.cc](https://zagent.aitun.cc)
- **PyPI**: [samai-zagent](https://pypi.org/project/samai-zagent/)

## 许可证 / License

专有软件，仅提供二进制分发。Proprietary software — binary distribution only.

---

联系方式 Contact: admin@samai.cc

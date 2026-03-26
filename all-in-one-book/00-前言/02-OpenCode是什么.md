# OpenCode 是什么

> 📌 OpenCode 是一个开源的 AI 编程代理（Coding Agent），让你在终端中与 AI 结对编程。

## 一句话定义

**OpenCode 是一个运行在终端里的 AI 编程助手**，它能理解你的代码库，帮你读代码、写代码、改代码、运行命令，就像一个坐在你旁边的资深程序员搭档。

## 核心特性

| 特性 | 说明 |
|------|------|
| 🤖 **多模型支持** | 支持 Claude、GPT、Gemini、Mistral 等 20+ 种 LLM |
| 🔧 **内置工具** | 文件读写、代码搜索、Shell 执行、Git 操作等 |
| 🔌 **MCP 协议** | 通过 Model Context Protocol 无限扩展工具能力 |
| 🖥️ **多端体验** | TUI 终端界面、Web 应用、桌面客户端 |
| 📂 **项目感知** | 自动理解项目结构、Git 状态、文件关系 |
| 🔒 **权限控制** | 精细的权限模型，控制 AI 可以做什么 |
| 🧩 **可扩展** | 自定义 Agent、Tool、Command、Plugin |
| 💾 **会话持久化** | 对话历史保存在本地 SQLite 数据库 |

## 与同类工具对比

| 特性 | OpenCode | GitHub Copilot CLI | Cursor | Aider |
|------|----------|-------------------|--------|-------|
| 开源 | ✅ MIT | ❌ | ❌ | ✅ |
| 多 LLM 支持 | ✅ 20+ | ❌ 仅 GPT | ❌ 有限 | ✅ |
| MCP 协议 | ✅ | ❌ | ✅ | ❌ |
| TUI 界面 | ✅ | ✅ | ❌ | ✅ |
| Web 界面 | ✅ | ❌ | ✅ | ❌ |
| 桌面客户端 | ✅ | ❌ | ✅ | ❌ |
| 插件系统 | ✅ | ❌ | ❌ | ❌ |
| 自定义 Agent | ✅ | ❌ | ❌ | ❌ |

## 项目背景

OpenCode 最初由 [anomalyco](https://github.com/anomalyco) 团队开发，本书基于 `propress/opencode` 仓库的 `dev` 分支编写。项目采用 MIT 许可证，欢迎社区贡献。

- **官网**: https://opencode.ai
- **GitHub**: https://github.com/anomalyco/opencode
- **技术栈**: TypeScript + Bun + Effect-TS + Vercel AI SDK + SolidJS + Tauri + Drizzle ORM

## OpenCode 能做什么？

```
你：帮我把 src/utils.ts 里的所有 forEach 改成 for...of 循环

OpenCode：
1. 🔍 搜索 src/utils.ts 中的 forEach 用法
2. 📖 读取文件内容，理解上下文
3. ✏️ 逐个替换为 for...of，保持语义一致
4. ✅ 展示修改 diff，等你确认
5. 💾 保存文件，创建 Git 快照
```

这就是 OpenCode 的核心工作方式：**理解意图 → 分析代码 → 选择工具 → 执行操作 → 确认结果**。

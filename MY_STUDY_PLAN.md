# AI Agents for Beginners - 7天学习计划

## 课程概况

微软官方 AI Agent 入门课程，共16课（01-18），核心框架：Microsoft Agent Framework (MAF) + Azure AI Foundry Agent Service V2。

## 推荐阅读顺序

1. 根目录 `README.md` — 课程总览
2. `00-course-setup/README.md` — 环境搭建
3. `STUDY_GUIDE.md` — 全课程知识点精华
4. 中文翻译版 `translations/zh-CN/README.md`（可选）
5. 按 `01` → `18` 顺序读每个 lesson 的 README

## 7天学习计划

| 天数 | 课程 | 重点 |
|---|---|---|
| **Day 1** | 00-setup + 01-intro + 02-frameworks | 环境搭建 + Agent 概念 + 框架概览 |
| **Day 2** | 03-design-patterns + 04-tool-use | 4种设计模式 + 工具调用 Notebook |
| **Day 3** | 05-agentic-rag + 06-trustworthy | RAG 检索增强 + 安全可信设计 |
| **Day 4** | 07-planning + 08-multi-agent | 规划模式 + 多Agent协作（核心难点） |
| **Day 5** | 09-metacognition + 10-production | 元认知反思 + 生产部署 |
| **Day 6** | 11-protocols + 12-context + 13-memory | MCP/A2A协议 + 上下文工程 + 记忆管理 |
| **Day 7** | 14-MAF + 15-browser + 18-security | MAF深入 + 浏览器Agent + 安全 |

每天约2-3小时：读README(30min) → 跑Notebook(1-2h) → 看视频(可选)

## 代码运行依赖

- **基本**：Python 3.12+, Azure账号, `az login`, `.env` 配置
- **Lesson 05**：额外需要 Azure AI Search
- **Lesson 06/08**：部分用 GitHub Models，需要 `GITHUB_TOKEN`
- **Lesson 08**：Bing Grounding 需要连接ID
- **Lesson 15**：需要 Playwright 浏览器环境
- **无Azure时**：可用 MiniMax 作为 OpenAI 兼容替代

## 同步上游更新

当微软更新了课程内容，执行以下命令获取更新：

```bash
# 1. 从微软原仓库下载更新（只下载到远程引用，不改变工作目录）
git fetch upstream

# 2. 合并到本地 main 分支
git merge upstream/main

# 3. 推到自己的 GitHub fork
git push origin main
```

| remote | 指向 |
|---|---|
| `origin` | 自己的 fork |
| `upstream` | 微软原仓库（microsoft/ai-agents-for-beginners） |

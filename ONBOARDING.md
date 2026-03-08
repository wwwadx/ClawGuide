# 新用户画像收集

当有新用户来问 "OpenClaw 能帮我做什么？" 时，使用这个模板了解他们的需求。

## 提问模板

```
你好！我是 OpenClaw 新手引导助手 🦞

OpenClaw 是一个个人 AI 助手，可以：
- 在你常用的聊天应用里回答问题（WhatsApp/Telegram/Discord/飞书等）
- 自动化重复性任务
- 连接你的工具和服务（GitHub、Notion、日历等）
- 通过自定义技能扩展功能

为了给你推荐最合适的用法，我想了解一下：

### 1. 你的日常工作/学习场景是什么？
（例如：软件工程师、学生、内容创作者、自由职业者等）

### 2. 你平时最常用哪些工具/平台？
（例如：GitHub、Notion、飞书、微信、Gmail 等）

### 3. 你有什么重复性任务希望自动化？
（例如：每天整理邮件、每周写报告、定时备份数据等）

### 4. 你希望 OpenClaw 在哪些方面帮你提升效率？
（例如：写作、编程、研究、生活管理等）

### 5. 你最常使用哪个聊天应用？
（我会帮你配置到那里）

回答这些问题后，我会：
1. 匹配你已经安装的工具相关的 skills
2. 推荐适合你的自动化场景
3. 提供具体的实现方案
4. 帮你一步步安装配置
```

## 场景匹配逻辑

### 如果用户是软件工程师
推荐：
- PR 审查自动化
- GitHub issue 管理
- 代码重构助手
- 技术文档生成

Skills needed:
- `github`
- `coding-agent`
- `summarize`

### 如果用户是内容创作者
推荐：
- 文章大纲生成
- SEO 优化建议
- 社交媒体发布
- 选题头脑风暴

Skills needed:
- `summarize`
- `tavily-search` (研究)
- `article` (如果可用)

### 如果用户是学生/研究者
推荐：
- 论文阅读笔记
- Flashcard 生成
- 文献综述
- 研究项目管理

Skills needed:
- `flashcards`
- `memory-system`
- `tavily-search`
- `notion` 或 `obsidian`

### 如果用户是自由职业者
推荐：
- 客户沟通记录
- 发票和账单管理
- 项目时间追踪
- 作品集维护

Skills needed:
- `feishu-doc` 或 `notion`
- `memory-system`

## 快速开始方案

### 方案 A：极简入门（5分钟）
```
1. 安装基础 skills：summarize, tavily-search
2. 连接一个聊天应用（例如 Telegram）
3. 测试："帮我总结这篇文章"
```

### 方案 B：开发者效率（15分钟）
```
1. 安装：github, coding-agent, summarize
2. 连接 GitHub
3. 设置 PR 审查自动化
```

### 方案 C：生活管理（10分钟）
```
1. 安装：memory-system, weather, feishu-doc
2. 设置每日提醒
3. 创建习惯追踪
```

## 对话示例

### 用户："我是程序员，想提高效率"
```
AI：太好了！我推荐几个适合程序员的用法：

1. PR 审查助手
   - 每次有新 PR 时自动审查
   - 在 Telegram/飞书给你反馈
   - 需要安装：github, coding-agent

2. 代码重构顾问
   - 描述需要重构的代码
   - 给出具体建议
   - 需要安装：coding-agent

3. 技术文档生成
   - 从代码自动生成注释
   - 生成 README
   - 需要安装：summarize

想先试哪一个？我可以帮你安装配置。
```

### 用户："我是学生，有很多论文要看"
```
AI：理解！论文阅读确实费时。我推荐：

1. 论文摘要助手
   - 上传 PDF，自动总结核心观点
   - 需要安装：summarize

2. 研究笔记系统
   - 自动保存重要摘录
   - 跨论文关联主题
   - 需要安装：memory-system, notion/obsidian

3. Flashcard 生成器
   - 从笔记自动生成复习卡片
   - 间隔重复提醒
   - 需要安装：flashcards

你平时用 Notion 还是 Obsidian 管理笔记？或者我可以推荐一个。
```

# OpenClaw 新手引导模板 🦞

> 5 分钟启动你的个人 AI 助手 - 专注于解答 "我能用 OpenClaw 做什么？"

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![OpenClaw](https://img.shields.io/badge/OpenClaw-latest-blue)](https://github.com/openclaw/openclaw)

---

## 🌐 语言 Language

[**English**](README.en.md) | **中文**

---

## 🌍 项目简介 / Project Overview

**[English](README.en.md) | [中文](README.md) (current)**

欢迎来到 ClawGuide！这是一个配置好的 OpenClaw workspace，帮助你快速上手个人 AI 助手。

**核心理念：** 🗣️ **用对话代替配置文件**

- 告诉助手你想要什么，它会自动完成
- 不需要手动编辑文件
- 10 分钟内体验 AI 自动化的价值

Welcome to ClawGuide! This is a configured OpenClaw workspace to help you quickly get started with your personal AI assistant.

**Core Philosophy:** 🗣️ **Customize through conversation, not config files**

- Tell the assistant what you want, it handles the rest
- No manual file editing needed
- Experience AI automation value within 10 minutes

---

## ✨ 这个项目是什么？

这是一个**配置好的 OpenClaw workspace**，专门用来帮助新用户快速上手。

**核心理念：** 🗣️ **用对话代替配置文件**

不需要懂代码或编辑配置文件，只需要：
- 告诉助手你想要什么
- 它会自己修改配置、安装 skills、调整行为
- 你只管提需求，剩下的交给 AI

**核心功能：**
- 🎯 **场景匹配** - 告诉我你的工作，我推荐合适的自动化方案
- 📚 **用例库** - 15+ 真实使用场景和配置教程
- 🔧 **即插即用** - Clone 后立即可用
- 🗣️ **对话式定制** - 用对话代替手动编辑
- 🚀 **持续更新** - 收集社区用例，不断完善

**不适合：**
- ❌ 寻找"最强大"配置的人
- ❌ 想深度定制的人（先用基础版再定制）
- ❌ 不愿尝试新工具的人

**适合：**
- ✅ 刚安装 OpenClaw 不知道做什么的人
- ✅ 想提升工作效率但不知道从哪开始的人
- ✅ 愿意花 10 分钟体验 AI 自动化的人
- ✅ **更喜欢对话而不是编辑文件的人** 🎯

---

## 🚀 5 分钟快速开始

### 前置要求

1. **已安装 OpenClaw**
   ```bash
   # 如果还没安装
   npm install -g openclaw@latest
   openclaw onboard --install-daemon
   ```

2. **已配置至少一个聊天渠道**（Telegram/WhatsApp/飞书等）

### 安装这个模板

```bash
# 1. Clone 这个仓库
git clone https://github.com/your-username/openclaw-starter-template.git
cd openclaw-starter-template

# 2. 设置为你的 workspace
openclaw workspace set $(pwd)

# 3. 重启 gateway
openclaw gateway restart
```

### 第一次对话

在你的聊天应用中说：

```
@your_bot 我是新用户，能帮我做什么？
```

你的助手会引导你了解可能的使用场景。

---

## 📖 使用场景

### 💼 开发者

| 场景 | 效果 | 配置时间 |
|------|------|----------|
| PR 自动审查 | 每个自动审查，Telegram 通知 | 15 分钟 |
| 代码重构顾问 | 描述问题，获得重构建议 | 10 分钟 |
| 技术文档生成 | 从代码生成注释和 README | 5 分钟 |

**详细教程：** 见 `SCENARIOS_QUICK_REF.md` - 开发者场景

---

### 📚 学生/研究者

| 场景 | 效果 | 配置时间 |
|------|------|----------|
| 论文阅读助手 | 自动总结 PDF，提取关键点 | 15 分钟 |
| Flashcard 生成 | 从笔记生成复习卡片 | 10 分钟 |
| 研究笔记系统 | 跨论文关联主题 | 20 分钟 |

**详细教程：** 见 `SCENARIOS_QUICK_REF.md` - 学习研究场景

---

### ✍️ 内容创作者

| 场景 | 效果 | 配置时间 |
|------|------|----------|
| 文章写作助手 | 选题、大纲、初稿自动生成 | 10 分钟 |
| PPT 生成器 | 从大纲生成幻灯片 | 15 分钟 |
| 图表绘制 | 文字描述自动生成流程图 | 5 分钟 |

**详细教程：** 见 `SCENARIOS_QUICK_REF.md` - 内容创作场景

---

### 🏠 生活自动化

| 场景 | 效果 | 配置时间 |
|------|------|----------|
| 智能购物清单 | 自动记录，自动下单 | 15 分钟 |
| 日程管理 | 自动添加会议，提前提醒 | 10 分钟 |
| 家居控制 | 语音控制设备，场景自动化 | 20 分钟 |

**详细教程：** 见 `SCENARIOS_QUICK_REF.md` - 生活自动化场景

---

## 📁 文件说明

```
openclaw-starter-template/
├── README.md                    # 本文件
├── QUICKSTART.md               # 5 分钟上手指南（即将推出）
├── CUSTOMIZATION.md            # 如何自定义（即将推出）
├── USE_CASES.md                # 完整用例集合（即将推出）
├── SCENARIOS_QUICK_REF.md      # 场景快速参考 ⭐
├── TUTORIALS.md                # 教程收集
├── ONBOARDING.md               # 新用户引导流程
├── TUTORIAL_TEMPLATE.md        # 教程写作模板
├── USE_CASE_COLLECTION.md      # 用例收集清单
├── OPEN_SOURCE_CHECKLIST.md    # 开源准备清单
├── AGENTS.md                   # Workspace 说明
├── SOUL.md                     # 助手的"灵魂"（行为指南）
├── IDENTITY.md                 # 助手的身份
├── USER.md                     # 用户信息模板
├── TOOLS.md                    # 工具配置
├── HEARTBEAT.md                # 心跳配置
├── skills/                     # 已安装的 skills
│   ├── agent-browser/          # 浏览器自动化
│   ├── ai-ppt-generator/       # PPT 生成
│   ├── baidu-search/           # 百度搜索
│   ├── diagram-generator/      # 图表生成
│   ├── find-skills/            # 查找 skills
│   ├── github/                 # GitHub 集成
│   ├── memory-system/          # 记忆系统
│   ├── pptx/                   # PowerPoint
│   ├── self-improving/         # 自我改进
│   ├── summarize/              # 文本摘要
│   ├── tencent-docs/           # 腾讯文档
│   ├── tencentcloud-lighthouse-skill/  # 腾讯云
│   └── tavily-search/          # 网络搜索
└── memory/                     # 记忆目录
    └── .gitkeep
```

---

## 🎯 核心文件说明

### SOUL.md - 助手的"灵魂"
定义了助手的行为准则和工作流程。这个助手的核心使命是**新手引导**。

### IDENTITY.md - 助手的身份
定义了助手的名字（ClawGuide）、性格和对话风格。

### SCENARIOS_QUICK_REF.md - 场景快速参考 ⭐
**最常用的文件！** 包含 15+ 个常见场景的快速匹配方案。

- 关键词索引
- 每个场景包含：描述、推荐方案、所需 skills、配置时间、效果

### ONBOARDING.md - 新用户引导
提问模板和对话示例，帮助快速理解用户需求。

### TUTORIALS.md - 教程收集
已收集的真实用例和教程链接。

---

## 🛠️ 自定义

这个模板只是一个起点。你可以通过**对话**或**编辑文件**来自定义。

### 🗣️ 方式一：直接对话（推荐！）

**跟你的 OpenClaw 助手说你想改什么，它会自己完成！**

```
# 修改身份
"把你的名字改成 '小助手'，用 🤖 做 emoji，风格要活泼一点"

# 调整行为
"我希望你回复时更简洁，不要用那么多表情符号"
"帮我写代码时要详细解释每一步"

# 添加功能
"帮我安装 weather skill"
"搜索一下有没有处理邮件的 skill"

# 记录用例
"我刚发现一个好用的场景：用 OpenClaw 自动整理浏览器书签，帮我记下来"
```

**优势：**
- ✅ 不需要了解文件结构
- ✅ 助手会自动编辑正确的文件
- ✅ 可以立即看到效果
- ✅ 更符合 AI 助手的交互方式

### 📝 方式二：手动编辑（可选）

如果你想精确控制或批量修改，也可以手动编辑：

#### 修改助手身份

编辑 `IDENTITY.md`：
```markdown
- **Name:** 改成你喜欢的名字
- **Emoji:** 换个更符合你风格的 emoji
- **Vibe:** 调整对话风格（正式/随意/幽默等）
```

#### 调整行为风格

编辑 `SOUL.md`：
```markdown
## Core Truths
# 添加或修改你希望助手遵循的原则
```

#### 添加新 Skills

```bash
# 搜索可用的 skills
skillhub search <关键词>

# 安装新 skill
skillhub install <skill-name>
```

#### 记录自己的用例

当发现新的使用场景时：
1. 更新 `SCENARIOS_QUICK_REF.md`
2. 添加到 `TUTORIALS.md`
3. （可选）写成完整教程

---

### 💡 推荐的工作流

**新用户：**
1. 先用**对话方式**体验和调整
2. 当熟悉后再手动微调

**进阶用户：**
1. 用对话快速迭代
2. 用编辑器批量修改
3. 两者结合使用

---

## 📚 进阶资源

### 官方文档
- [OpenClaw 官方文档](https://docs.openclaw.ai)
- [GitHub 仓库](https://github.com/openclaw/openclaw)
- [Discord 社区](https://discord.gg/clawd)

### 学习路径
1. **新手** → 阅读 `SCENARIOS_QUICK_REF.md`
2. **进阶** → 自定义 `IDENTITY.md` 和 `SOUL.md`
3. **专家** → 创建新 skills，贡献教程

---

## 🤝 贡献

欢迎贡献！

### 如何贡献

1. **报告问题** - [提交 Issue](../../issues)
2. **改进文档** - [提交 PR](../../pulls)
3. **分享用例** - 在 Discussions 分享你的场景

### 贡献指南

见 `OPEN_SOURCE_CHECKLIST.md` 中的 `CONTRIBUTING.md` 部分。

---

## 📝 更新日志

### v0.1.0 (2026-03-08)
- ✨ 初始版本
- 📚 15+ 场景用例
- 🎯 新手引导流程
- 🔧 13 个预装 skills
- 📖 完整文档模板

---

## 📄 许可证

MIT License - 详见 [LICENSE](LICENSE)

---

## 🙏 致谢

- OpenClaw 团队和社区
- 所有贡献用例的用户
- Discord #showcase 频道的分享者

---

## 💬 反馈

有问题或建议？

- 📮 [提交 Issue](../../issues)
- 💬 [Discord](https://discord.gg/clawd)
- ✉️ 联系：[你的联系方式]

---

**用 [OpenClaw](https://openclaw.ai) 构建 🦞**

_让每个人都拥有自己的 AI 助手_

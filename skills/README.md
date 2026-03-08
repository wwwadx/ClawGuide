# Skills 目录

> 这个 workspace 推荐使用的 skills

## 📋 关于这个目录

**重要：** skills **不会**包含在这个仓库中。你需要自己安装它们。

原因：
- Skills 通常安装在全局位置（`~/.openclaw/workspace/skills/`）
- 不同用户的安装路径不同
- Skills 会持续更新，应该安装最新版本

## 🚀 快速安装

### 安装所有推荐的 skills

```bash
# 使用 skillhub（推荐，CN 优化）
skillhub install summarize
skillhub install tavily-search
skillhub install memory-system
skillhub install github
skillhub install pptx
skillhub install diagram-generator
skillhub install baidu-search
skillhub install ai-ppt-generator

# 或使用 clawhub（公共注册表）
clawhub install summarize
clawhub install tavily-search
# ... 等等
```

### 按需安装

根据你的使用场景安装，见 [README.md](../README.md#-使用场景) 的场景列表。

## 📚 Core Skills（推荐安装）

| Skill | 用途 | 场景 |
|-------|------|------|
| `summarize` | 文本摘要 | 文章总结、会议纪要、论文阅读 |
| `tavily-search` | 网络搜索 | 研究话题、查找信息 |
| `memory-system` | 记忆管理 | 记录重要信息、长期知识 |
| `github` | GitHub 集成 | PR 审查、代码管理 |
| `pptx` | PowerPoint | PPT 生成、演示文稿 |
| `diagram-generator` | 图表生成 | 流程图、架构图 |
| `agent-browser` | 浏览器自动化 | 网页操作、数据抓取 |
| `self-improving` | 自我改进 | 持续学习和优化 |
| `find-skills` | 查找 skills | 发现新功能 |

## 🎯 按场景安装

### 开发者
```bash
skillhub install github
skillhub install coding-agent  # 如果可用
```

### 学生/研究者
```bash
skillhub install summarize
skillhub install memory-system
skillhub install flashcards  # 如果可用
```

### 内容创作者
```bash
skillhub install pptx
skillhub install ai-ppt-generator
skillhub install diagram-generator
```

### 生活自动化
```bash
skillhub install agent-browser
skillhub install weather
```

## 🔍 搜索更多 skills

```bash
# 搜索关键词
skillhub search <关键词>

# 列出已安装的 skills
skillhub list

# 或使用 clawhub
clawhub search <关键词>
```

## 📖 参考

- [OpenClaw Skills 文档](https://docs.openclaw.ai/skills)
- [SkillHub (CN 优化)](https://clawhub.com)
- [场景快速参考](../SCENARIOS_QUICK_REF.md)

## 💡 提示

安装 skills 后，重启 OpenClaw Gateway：
```bash
openclaw gateway restart
```

# ClawGuide: OpenClaw Onboarding Template 🦞

> Get your personal AI assistant running in 5 minutes - Focused on answering "What can I do with OpenClaw?"

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![OpenClaw](https://img.shields.io/badge/OpenClaw-latest-blue)](https://github.com/openclaw/openclaw)

---

## 🌐 Language

[**English**](README.md) | [中文文档](README.zh-CN.md)

---

## ✨ What is this?

This is a **configured OpenClaw workspace** designed to help new users get started quickly.

**Core Philosophy:** 🗣️ **Customize through conversation, not config files**

Instead of editing configuration files, just:
- Tell the assistant what you want
- It will modify configs, install skills, and adjust behavior automatically
- You just state requirements, let AI handle the rest

**Key Features:**
- 🎯 **Scenario Matching** - Tell me your work, I'll recommend automation solutions
- 📚 **Use Case Library** - 15+ real-world scenarios and setup tutorials
- 🔧 **Plug & Play** - Clone and use immediately
- 🗣️ **Conversational Customization** - Customize via chat, not file editing
- 🚀 **Continuously Updated** - Collecting community use cases

**Not for:**
- ❌ People looking for the "most powerful" config
- ❌ People who want deep customization (start with basic first)
- ❌ People unwilling to try new tools

**Perfect for:**
- ✅ New OpenClaw users wondering what to do
- ✅ People wanting to boost productivity but don't know where to start
- ✅ Anyone willing to spend 10 minutes experiencing AI automation
- ✅ **People who prefer conversation over editing files** 🎯

---

## 🚀 5-Minute Quick Start

### Prerequisites

1. **OpenClaw installed**
   ```bash
   # If not installed yet
   npm install -g openclaw@latest
   openclaw onboard --install-daemon
   ```

2. **At least one chat channel configured** (Telegram/WhatsApp/Feishu/etc.)

### Install this template

```bash
# 1. Clone this repository
git clone https://github.com/wwwadx/ClawGuide.git
cd ClawGuide

# 2. Set as your workspace
openclaw workspace set $(pwd)

# 3. Restart gateway
openclaw gateway restart
```

### First Conversation

In your chat app, say:

```
@your_bot I'm a new user, what can you help me with?
```

Your assistant will guide you through possible use cases.

---

## 📖 Use Cases

### 💼 Developers

| Scenario | Effect | Setup Time |
|----------|--------|------------|
| PR Auto-Review | Auto-review every PR, Telegram notification | 15 min |
| Code Refactoring Advisor | Describe problem, get refactoring suggestions | 10 min |
| Technical Documentation | Generate comments and README from code | 5 min |

**Detailed guide:** See `SCENARIOS_QUICK_REF.zh-CN.md` - Developer Scenarios

---

### 📚 Students/Researchers

| Scenario | Effect | Setup Time |
|----------|--------|------------|
| Paper Reading Assistant | Auto-summarize PDFs, extract key points | 15 min |
| Flashcard Generator | Generate review cards from notes | 10 min |
| Research Notes System | Cross-paper topic linking | 20 min |

**Detailed guide:** See `SCENARIOS_QUICK_REF.zh-CN.md` - Learning & Research

---

### ✍️ Content Creators

| Scenario | Effect | Setup Time |
|----------|--------|------------|
| Article Writing Assistant | Topics, outlines, drafts auto-generated | 10 min |
| PPT Generator | Generate slides from outlines | 15 min |
| Diagram Creation | Generate flowcharts from text descriptions | 5 min |

**Detailed guide:** See `SCENARIOS_QUICK_REF.zh-CN.md` - Content Creation

---

### 🏠 Life Automation

| Scenario | Effect | Setup Time |
|----------|--------|------------|
| Smart Shopping List | Auto-track, auto-order | 15 min |
| Schedule Management | Auto-add meetings, advance reminders | 10 min |
| Home Control | Voice control, scene automation | 20 min |

**Detailed guide:** See `SCENARIOS_QUICK_REF.zh-CN.md` - Life Automation

---

## 📁 File Structure

```
ClawGuide/
├── README.md                    # This file
├── README.zh-CN.md              # 中文文档 ⭐
├── QUICKSTART.md               # 5-minute guide (coming soon)
├── CUSTOMIZATION.md            # How to customize (coming soon)
├── USE_CASES.md                # Complete use case collection (coming soon)
├── SCENARIOS_QUICK_REF.md      # Scenario quick reference ⭐
├── SCENARIOS_QUICK_REF.zh-CN.md
├── TUTORIALS.md                # Tutorial collection
├── TUTORIALS.zh-CN.md
├── ONBOARDING.md               # New user onboarding flow
├── ONBOARDING.zh-CN.md
├── CONVERSATION_EXAMPLES.md    # Conversational customization examples
├── CONVERSATION_EXAMPLES.zh-CN.md
├── TUTORIAL_TEMPLATE.md        # Tutorial writing template
├── USE_CASE_COLLECTION.md      # Use case collection checklist
├── OPEN_SOURCE_CHECKLIST.md    # Open source preparation
├── PROJECT_SUMMARY.md          # Project completion summary
├── AGENTS.md                   # Workspace description
├── SOUL.md                     # Assistant's "soul" (behavior guidelines)
├── IDENTITY.md                 # Assistant identity
├── USER.md                     # User info template
├── TOOLS.md                    # Tools config
├── HEARTBEAT.md                # Heartbeat config
├── skills/                     # Installed skills
│   └── README.md               # Skills installation guide
└── memory/                     # Memory directory
    └── .gitkeep
```

---

## 🛠️ Customization

This template is just a starting point. You can customize via **conversation** or **file editing**.

### 🗣️ Method 1: Direct Conversation (Recommended!)

**Just tell your OpenClaw assistant what you want to change, it will do it!**

```
# Modify identity
"Change your name to 'Assistant', use 🤖 as emoji, be more lively"

# Adjust behavior
"I prefer more concise responses, fewer emojis"
"Explain each step when helping me write code"

# Add features
"Install weather skill for me"
"Search for email processing skills"

# Record use cases
"Just found a great scenario: auto-organize browser bookmarks with OpenClaw, please record this"
```

**Advantages:**
- ✅ No need to understand file structure
- ✅ Assistant auto-edits correct files
- ✅ Immediate effect
- ✅ More aligned with AI assistant interaction

### 📝 Method 2: Manual Editing (Optional)

If you want precise control or batch modifications:

#### Modify Assistant Identity

Edit `IDENTITY.md`:
```markdown
- **Name:** Change to preferred name
- **Emoji:** Change emoji matching your style
- **Vibe:** Adjust conversation style (formal/casual/humorous/etc.)
```

#### Adjust Behavior Style

Edit `SOUL.md`:
```markdown
## Core Truths
# Add or modify principles you want the assistant to follow
```

#### Add New Skills

```bash
# Search available skills
skillhub search <keyword>

# Install new skill
skillhub install <skill-name>
```

#### Record Your Use Cases

When discovering new scenarios:
1. Update `SCENARIOS_QUICK_REF.zh-CN.md`
2. Add to `TUTORIALS.zh-CN.md`
3. (Optional) Write complete tutorial

---

### 💡 Recommended Workflow

**New Users:**
1. Start with **conversation method** to experience and adjust
2. Manually fine-tune when familiar

**Advanced Users:**
1. Use conversation for quick iteration
2. Use editor for batch modifications
3. Combine both approaches

---

## 🌐 Language Support

**Documentation available in:**
- 🇬🇧 [English](README.md) (Default)
- 🇨🇳 [中文](README.zh-CN.md)

**Configuration files (SOUL.md, IDENTITY.md, USER.md):**
- Keep in Chinese (these are for your assistant, not for reading)

---

## 📚 Advanced Resources

### Official Documentation
- [OpenClaw Official Docs](https://docs.openclaw.ai)
- [GitHub Repository](https://github.com/openclaw/openclaw)
- [Discord Community](https://discord.gg/clawd)

### Learning Path
1. **Beginner** → Read `SCENARIOS_QUICK_REF.zh-CN.md`
2. **Intermediate** → Customize `IDENTITY.md` and `SOUL.md`
3. **Expert** → Create new skills, contribute tutorials

---

## 🤝 Contributing

Contributions welcome!

### How to Contribute

1. **Report Issues** - [Submit Issue](../../issues)
2. **Improve Docs** - [Submit PR](../../pulls)
3. **Share Use Cases** - Share scenarios in Discussions

### Contribution Guide

See `OPEN_SOURCE_CHECKLIST.md` - Contributing section.

---

## 📝 Changelog

### v0.1.0 (2026-03-08)
- ✨ Initial release
- 📚 15+ scenario use cases
- 🎯 Newbie onboarding flow
- 🔧 13 pre-installed skills
- 📖 Complete documentation templates
- 🗣️ Conversational customization emphasis
- 🌐 Bilingual support (EN/ZH)

---

## 📄 License

MIT License - See [LICENSE](LICENSE)

---

## 🙏 Acknowledgments

- OpenClaw team and community
- All users contributing use cases
- Sharers in Discord #showcase channel

---

## 💬 Feedback

Questions or suggestions?

- 📮 [Submit Issue](../../issues)
- 💬 [Discord](https://discord.gg/clawd)
- ✉️ Contact: [Your contact info]

---

**Built with [OpenClaw](https://openclaw.ai) 🦞**

_Everyone deserves their own AI assistant_

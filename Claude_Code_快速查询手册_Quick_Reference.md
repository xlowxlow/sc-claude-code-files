# 🚀 Claude Code 快速查询手册 | Quick Reference Guide

> 一页纸掌握Claude Code核心功能 | Master Claude Code on one page

---

## 📋 常用命令速查 | Command Quick Reference

| 命令 Command | 功能 Function | 快捷键 Shortcut | 使用场景 Use Case |
|--------------|---------------|-----------------|-------------------|
| `/init` | 初始化项目，创建CLAUDE.md | - | 新项目开始 |
| `/clear` | 清空对话历史 | - | 切换任务 |
| `/compact` | 压缩对话，保留关键信息 | - | 节省token |
| `/cost` | 查看当前费用 | - | 监控支出 |
| `/mcp` | 管理MCP服务器 | - | 连接外部工具 |
| `/help` | 获取帮助 | - | 遇到问题时 |
| `#` | 添加项目记忆 | - | 记录重要信息 |
| `@文件名` | 引用特定文件 | - | 指定操作目标 |
| `ESC` | 中断当前操作 | `Esc` | 需要停止时 |
| `ESC ESC` | 回退到之前状态 | `Esc`×2 | 撤销操作 |
| `exit` | 退出Claude Code | - | 结束会话 |
| `!命令` | 执行bash命令 | - | 系统操作 |

## 🎯 模式切换 | Mode Switching

| 模式 Mode | 切换方式 Switch | 特点 Features | 适用 Suitable For |
|-----------|----------------|---------------|-------------------|
| **计划模式** Plan | `Shift+Tab` | 先展示计划，需确认 | 重要改动 |
| **自动执行** Auto | `Shift+Tab` | 直接执行操作 | 明确任务 |
| **深度思考** Think | 添加`think` | 深入分析问题 | 复杂问题 |

## 💡 Prompt模板库 | Prompt Templates

### 🔍 理解代码 | Understanding Code
```
给我@文件名的概览，用简单语言解释
Give me overview of @filename in simple terms

解释这个功能是如何工作的
Explain how this feature works

画出这个系统的架构图
Draw the architecture diagram of this system
```

### ✨ 添加功能 | Adding Features
```
添加[功能名]，要求：
1. [需求1]
2. [需求2]
一步步实现并解释

Add [feature], requirements:
1. [requirement 1]
2. [requirement 2]
Implement step by step with explanations
```

### 🐛 调试修复 | Debug & Fix
```
我遇到错误：[错误信息]
请定位问题并修复

I got error: [error message]
Please locate and fix the issue

写测试来验证这个修复
Write tests to verify this fix
```

### 🔄 代码重构 | Refactoring
```
重构@文件名：
- 提取重复代码
- 改善命名
- 添加类型注解

Refactor @filename:
- Extract duplicate code
- Improve naming
- Add type annotations
```

## 🧠 思考级别 | Thinking Levels

```
普通任务 → 不需要think
Normal task → No think needed

中等复杂 → think
Medium complexity → think

复杂问题 → think hard
Complex problem → think hard

极复杂 → think harder
Very complex → think harder

终极挑战 → ultrathink
Ultimate challenge → ultrathink
```

## 🔌 MCP服务器快速配置 | MCP Server Quick Setup

### Playwright (浏览器自动化 | Browser Automation)
```bash
claude mcp add playwright npx @playwright/mcp@latest
```

### Figma (设计导入 | Design Import)
```bash
# 官方版 Official
claude mcp add --transport http figma-dev http://127.0.0.1:3845/mcp

# 免费版 Free
claude mcp add framelink npx -y figma-developer-mcp --figma-api-key=KEY --stdio
```

## 🌳 Git Worktrees 并行开发 | Parallel Development

```bash
# 创建worktree | Create worktree
git worktree add .trees/feature-name

# 在worktree中启动Claude | Launch Claude in worktree
cd .trees/feature-name && claude

# 合并所有worktrees | Merge all worktrees
git merge .trees/*/main
```

## 📝 项目初始化最佳实践 | Project Init Best Practices

```bash
# 1. 创建项目 | Create project
mkdir my-project && cd my-project

# 2. 启动Claude | Launch Claude
claude

# 3. 初始化 | Initialize
/init

# 4. 添加项目特定信息 | Add project specifics
#使用TypeScript和React
#数据库是PostgreSQL
#所有API需要JWT认证

# 5. 开始开发 | Start developing
创建一个用户认证系统
Create a user authentication system
```

## 🎮 快捷操作组合 | Quick Operation Combos

### 快速原型 | Rapid Prototyping
```
1. claude
2. 创建[应用描述] → Create [app description]
3. Shift+Tab (自动模式 auto mode)
4. 直接看结果 | See results directly
```

### 复杂调试 | Complex Debugging
```
1. ESC (停止当前 stop current)
2. think hard
3. 描述问题 | Describe problem
4. 等待深度分析 | Wait for deep analysis
```

### 并行开发 | Parallel Development
```
1. git worktree add .trees/feature1
2. git worktree add .trees/feature2
3. 分别启动Claude | Launch Claude separately
4. 同时开发 | Develop simultaneously
```

## 💰 费用控制技巧 | Cost Control Tips

| 技巧 Tip | 说明 Description | 节省 Savings |
|----------|-----------------|--------------|
| 使用`@文件` | 精确指定文件，避免全局扫描 | ~30% |
| 定期`/compact` | 压缩对话历史 | ~40% |
| 计划模式 | 避免错误重做 | ~20% |
| 维护CLAUDE.md | 减少重复解释 | ~25% |

## ⚠️ 常见错误速查 | Common Errors Quick Fix

| 错误 Error | 原因 Cause | 解决 Solution |
|-----------|------------|---------------|
| `command not found` | 未安装Claude Code | `npm install -g @anthropic-ai/claude-code` |
| `token limit exceeded` | 对话过长 | `/compact` 或 `/clear` |
| `MCP connection failed` | 服务器未启动 | 重新添加MCP服务器 |
| `query failed` | API配置错误 | 检查.env文件和API密钥 |

## 🔥 高频使用场景 | High-Frequency Scenarios

### 1. 创建新项目 | Create New Project
```
claude → /init → 描述需求 → 自动生成
claude → /init → describe needs → auto generate
```

### 2. 理解现有代码 | Understand Existing Code
```
给我项目概览 → 解释@核心文件 → 画架构图
Give overview → Explain @core-file → Draw diagram
```

### 3. 添加新功能 | Add New Feature
```
Shift+Tab(计划模式) → 描述功能 → 确认 → 执行
Shift+Tab(plan mode) → describe feature → confirm → execute
```

### 4. 修复Bug | Fix Bug
```
粘贴错误 → think → 自动定位修复 → 写测试
Paste error → think → auto locate & fix → write test
```

### 5. 优化性能 | Optimize Performance
```
分析@文件性能 → think hard → 获取优化方案 → 实施
Analyze @file performance → think hard → get optimization → implement
```

## 📌 记住这些就够了 | Just Remember These

### 最常用的5个命令 | Top 5 Commands
1. `/init` - 项目开始 | Project start
2. `/clear` - 清理重启 | Clean restart
3. `@文件` - 指定目标 | Specify target
4. `ESC` - 紧急停止 | Emergency stop
5. `#` - 添加记忆 | Add memory

### 最有用的3个技巧 | Top 3 Tips
1. 具体明确的提示词 | Specific prompts
2. 使用`@`引用文件 | Use @ for files
3. 适时使用think | Use think wisely

### 最省钱的3个方法 | Top 3 Money Savers
1. `/compact`压缩对话 | Compact conversation
2. 精确指定文件 | Specify files precisely
3. 维护CLAUDE.md | Maintain CLAUDE.md

---

> 💡 **Pro Tip**: 打印此页放在手边，快速查询不迷路！
> 
> Print this page and keep it handy for quick reference!

**需要更多帮助？| Need more help?** 
- 输入 `/help` 
- 查看完整教程 `Claude_Code_完整教程_Complete_Guide.md`
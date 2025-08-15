# 📚 Claude Code 完整教程与使用手册 | Complete Guide & User Manual

> 🌟 **本教程特色 | Features**：
> - 🌐 中英双语对照 | Chinese-English Bilingual
> - 🔰 初学者友好 | Beginner Friendly  
> - 📖 专业术语详解 | Technical Terms Explained
> - 💡 实战案例驱动 | Practice-Driven Examples

---

## 📑 目录 | Table of Contents

- [第0章：基础概念](#第0章基础概念--chapter-0-basic-concepts)
- [第1章：快速入门](#第1章快速入门--chapter-1-quick-start)
- [第2章：核心命令详解](#第2章核心命令详解--chapter-2-core-commands)
- [第3章：实战Prompts集锦](#第3章实战prompts集锦--chapter-3-practical-prompts)
- [第4章：高级功能](#第4章高级功能--chapter-4-advanced-features)
- [第5章：项目实战案例](#第5章项目实战案例--chapter-5-real-projects)
- [第6章：常见问题解答](#第6章常见问题解答--chapter-6-faq)
- [附录：专业术语词汇表](#附录专业术语词汇表--appendix-glossary)

---

## 第0章：基础概念 | Chapter 0: Basic Concepts

### 🤖 什么是Claude Code？| What is Claude Code?

Claude Code 是 Anthropic 公司开发的**AI编程助手**（AI Coding Assistant），它是一个高度智能化的编程工具，能够理解自然语言并自动生成代码。

> 💡 **初学者理解 | Beginner's Understanding**：
> 想象Claude Code是你的编程搭档，你用日常语言告诉它想做什么，它就能帮你写出相应的程序代码，就像有一个经验丰富的程序员坐在你旁边一样。
> 
> Imagine Claude Code as your programming partner. You tell it what you want in everyday language, and it writes the code for you, like having an experienced programmer sitting next to you.

> 🎯 **专业定义 | Professional Definition**：
> Claude Code 是基于大语言模型（LLM）的代码生成、理解和优化系统，通过自然语言处理（NLP）技术实现人机交互，支持多种编程语言和开发框架。
> 
> Claude Code is a code generation, understanding, and optimization system based on Large Language Models (LLM), implementing human-computer interaction through Natural Language Processing (NLP) technology, supporting multiple programming languages and development frameworks.

### 🎯 核心能力 | Core Capabilities

| 能力 | Capability | 说明 | Description | 示例 | Example |
|------|------------|------|-------------|------|---------|
| 🔍 代码理解 | Code Understanding | 分析现有代码结构和逻辑 | Analyze existing code structure and logic | "解释这个函数的作用" | "Explain what this function does" |
| ✍️ 代码生成 | Code Generation | 根据需求自动编写代码 | Automatically write code based on requirements | "创建一个登录页面" | "Create a login page" |
| 🐛 调试修复 | Debug & Fix | 找出并修复代码错误 | Find and fix code errors | "修复这个报错" | "Fix this error" |
| 🔄 代码重构 | Code Refactoring | 优化代码结构和性能 | Optimize code structure and performance | "重构这个函数使其更高效" | "Refactor this function to be more efficient" |
| 📝 文档生成 | Documentation | 自动生成代码文档 | Auto-generate code documentation | "为这个类添加文档" | "Add documentation for this class" |

### 🌟 为什么选择Claude Code？| Why Choose Claude Code?

**对于初学者 | For Beginners**：
- ✅ 无需记忆复杂语法 | No need to memorize complex syntax
- ✅ 实时学习编程知识 | Learn programming in real-time
- ✅ 快速实现想法 | Quickly implement ideas

**对于专业开发者 | For Professional Developers**：
- ✅ 提高开发效率 | Increase development efficiency
- ✅ 减少重复工作 | Reduce repetitive work
- ✅ 探索最佳实践 | Explore best practices

---

## 第1章：快速入门 | Chapter 1: Quick Start

### 📦 1.1 安装指南 | Installation Guide

#### 方法1：NPM安装（推荐）| Method 1: NPM Installation (Recommended)

```bash
# 步骤1：安装Node.js | Step 1: Install Node.js
# 访问 https://nodejs.org 下载安装 | Visit https://nodejs.org to download

# 步骤2：安装Claude Code | Step 2: Install Claude Code
npm install -g @anthropic-ai/claude-code

# 步骤3：验证安装 | Step 3: Verify installation
claude --version
```

> 💡 **名词解释 | Term Explanation**：
> - **NPM**：Node Package Manager，Node.js的包管理器，用于安装和管理JavaScript软件包
> - **-g**：global的缩写，表示全局安装，安装后可在任何位置使用

#### 方法2：VS Code集成 | Method 2: VS Code Integration

1. **打开VS Code | Open VS Code**
2. **打开项目文件夹 | Open project folder**
   - 文件 → 打开文件夹 | File → Open Folder
3. **打开终端 | Open terminal**
   - 终端 → 新建终端 | Terminal → New Terminal
   - 快捷键：`` Ctrl+` `` (Windows/Linux) 或 | or `` Cmd+` `` (Mac)
4. **输入命令 | Type command**：`claude`
5. **自动安装扩展 | Extension auto-installs**

> ⚠️ **注意事项 | Note**：
> 如果出现"command not found"错误，确保已安装Node.js和npm
> If you see "command not found" error, ensure Node.js and npm are installed

### 🚀 1.2 第一个项目 | Your First Project

#### 示例1：创建个人主页 | Example 1: Create Personal Homepage

```bash
# 1. 创建项目文件夹 | Create project folder
mkdir my-homepage
cd my-homepage

# 2. 启动Claude Code | Launch Claude Code
claude

# 3. 输入你的需求 | Enter your requirement
```

**中文提示示例 | Chinese Prompt Example**：
```
创建一个个人主页，包含：
1. 顶部导航栏
2. 个人简介部分
3. 技能展示
4. 联系方式
使用现代化设计，响应式布局
```

**English Prompt Example**：
```
Create a personal homepage with:
1. Top navigation bar
2. Personal introduction section
3. Skills showcase
4. Contact information
Use modern design with responsive layout
```

**Claude Code 会自动 | Claude Code will automatically**：
- ✅ 创建 `index.html` - 网页结构 | webpage structure
- ✅ 创建 `styles.css` - 样式设计 | styling design
- ✅ 创建 `script.js` - 交互功能 | interactive features
- ✅ 解释每部分代码的作用 | explain each part of the code

### 🎮 1.3 基本交互方式 | Basic Interaction Methods

#### 自然语言对话 | Natural Language Dialogue

```markdown
你 | You: 帮我创建一个待办事项应用
         Help me create a todo list app

Claude: 我来帮您创建一个待办事项应用。这个应用将包含添加、删除和标记完成功能。
        I'll help you create a todo list app with add, delete, and mark complete features.

        [自动生成代码... | Auto-generating code...]
```

#### 引用文件 | Reference Files

使用 `@` 符号引用特定文件 | Use `@` symbol to reference specific files：

```markdown
你 | You: 请优化 @index.html 的性能
         Please optimize @index.html performance

Claude: 我来分析并优化 index.html 文件...
        Let me analyze and optimize the index.html file...
```

### 💰 1.4 费用说明 | Cost Information

| 订阅类型 | Subscription Type | 价格 | Price | 适合人群 | Suitable For |
|---------|-------------------|------|--------|----------|--------------|
| Pro | 专业版 | $20/月 | $20/month | 个人开发者、学习者 | Individual developers, learners |
| Max | 高级版 | $100/月 | $100/month | 专业团队、频繁使用 | Professional teams, frequent users |
| API使用 | API Usage | 按量计费 | Pay as you go | 灵活使用 | Flexible usage |

> 💡 **费用监控 | Cost Monitoring**：
> 使用 `/cost` 命令查看当前会话费用 | Use `/cost` command to check current session cost

---

## 第2章：核心命令详解 | Chapter 2: Core Commands

### 📝 2.1 项目管理命令 | Project Management Commands

#### `/init` - 初始化项目 | Initialize Project

**作用 | Function**：
扫描整个代码库，创建 `CLAUDE.md` 文件，让Claude Code理解你的项目结构。
Scans the entire codebase and creates a `CLAUDE.md` file to help Claude Code understand your project structure.

**使用场景 | Use Cases**：
- 🆕 新项目开始时 | When starting a new project
- 📁 项目结构变化后 | After project structure changes
- 📝 需要Claude记住特定规则时 | When Claude needs to remember specific rules

**示例对话 | Example Dialogue**：
```
你 | You: /init

Claude: 正在分析您的代码库... | Analyzing your codebase...
        
        发现以下结构 | Found the following structure:
        - Python项目，使用FastAPI框架 | Python project using FastAPI framework
        - 包含测试文件 | Contains test files
        - 使用PostgreSQL数据库 | Uses PostgreSQL database
        
        已创建CLAUDE.md文件，包含项目关键信息 | Created CLAUDE.md with key project information
```

#### `/clear` - 清空对话 | Clear Conversation

**作用 | Function**：
清除当前对话历史，释放内存，重新开始。
Clear current conversation history, free memory, start fresh.

**使用场景 | Use Cases**：
- 🔄 切换到新任务 | Switching to new task
- 💾 内存占用过多 | Memory usage too high
- 🆕 需要全新上下文 | Need fresh context

#### `/compact` - 压缩对话 | Compact Conversation

**作用 | Function**：
保留关键信息，压缩对话历史，节省token使用。
Preserve key information, compress conversation history, save token usage.

**示例 | Example**：
```
你 | You: /compact

Claude: 已压缩对话历史。保留了以下关键信息：
        Compressed conversation history. Preserved key information:
        - 项目是电商网站 | Project is e-commerce website
        - 已完成用户认证模块 | Completed user authentication module
        - 当前任务：添加购物车功能 | Current task: Add shopping cart feature
```

#### `#` - 快速添加记忆 | Quick Add Memory

**作用 | Function**：
快速添加项目特定信息到Claude的记忆中。
Quickly add project-specific information to Claude's memory.

**示例 | Examples**：
```
# 项目使用uv管理Python依赖
# Project uses uv for Python dependency management

# 数据库有两个主要表：users和products
# Database has two main tables: users and products

# 所有API都需要JWT认证
# All APIs require JWT authentication
```

### 🎮 2.2 交互控制命令 | Interaction Control Commands

#### `ESC` - 中断操作 | Interrupt Operation

**作用 | Function**：
立即停止Claude的当前操作，可以重新引导。
Immediately stop Claude's current operation, can redirect.

**使用场景 | Use Cases**：
- ❌ Claude理解错误 | Claude misunderstood
- 🔄 需要改变方向 | Need to change direction
- ⏸️ 暂停执行 | Pause execution

#### `ESC ESC` - 回退对话 | Rewind Conversation

**作用 | Function**：
回退到之前的对话点，撤销最近的操作。
Rewind to previous conversation point, undo recent operations.

**示例场景 | Example Scenario**：
```
你：添加用户登录功能
You: Add user login feature
[Claude生成代码... | Claude generates code...]

你：ESC ESC
You: ESC ESC
[回退到生成代码前 | Rewinds to before code generation]

你：先添加注册功能
You: Add registration feature first
```

### 🛠️ 2.3 模式切换命令 | Mode Switching Commands

#### `Shift + Tab` - 切换执行模式 | Switch Execution Mode

**两种模式 | Two Modes**：

1. **计划模式 | Planning Mode** 🤔
   - Claude先展示计划，需确认后执行
   - Claude shows plan first, needs confirmation to execute
   - 适合：重要改动、不确定的操作
   - Suitable for: Important changes, uncertain operations

2. **自动执行模式 | Auto-Execute Mode** ⚡
   - Claude直接执行操作
   - Claude executes directly
   - 适合：明确任务、信任的操作
   - Suitable for: Clear tasks, trusted operations

### 📊 2.4 信息查询命令 | Information Query Commands

#### `/cost` - 查看费用 | Check Cost

```
你 | You: /cost

Claude: 当前会话费用 | Current session cost:
        - 输入tokens | Input tokens: 15,234
        - 输出tokens | Output tokens: 8,456
        - 预计费用 | Estimated cost: $0.47
```

#### `/mcp` - MCP服务器管理 | MCP Server Management

**作用 | Function**：
管理和查看已连接的MCP（Model Context Protocol）服务器。
Manage and view connected MCP (Model Context Protocol) servers.

**示例 | Example**：
```
你 | You: /mcp

Claude: 已连接的MCP服务器 | Connected MCP servers:
        1. playwright - 浏览器自动化 | Browser automation
        2. figma-dev - Figma设计导入 | Figma design import
        
        使用 'claude mcp add' 添加新服务器
        Use 'claude mcp add' to add new servers
```

---

## 第3章：实战Prompts集锦 | Chapter 3: Practical Prompts

### 🔍 3.1 代码理解类 | Code Understanding

#### 基础模板 | Basic Templates

**获取项目概览 | Get Project Overview**：
```
中文：给我这个项目的整体架构说明，包括主要模块和它们的关系
English: Give me an overview of this project's architecture, including main modules and their relationships
```

**理解特定功能 | Understand Specific Feature**：
```
中文：解释 @文件名 中的 [功能名] 是如何工作的，用简单语言说明
English: Explain how [feature name] in @filename works in simple terms
```

#### 实战示例 | Practical Example

**场景：理解RAG聊天机器人代码 | Scenario: Understanding RAG Chatbot Code**

```markdown
你 | You: 
请解释这个RAG聊天机器人的工作流程，从用户输入问题到得到答案的全过程
Explain the workflow of this RAG chatbot, from user input to getting answer

Claude的回答结构 | Claude's Response Structure:
1. 📥 接收用户输入 | Receive user input
   - 前端捕获用户问题 | Frontend captures user question
   - 发送到后端API | Send to backend API

2. 🔍 向量搜索 | Vector Search
   - 问题转换为向量 | Convert question to vector
   - 在ChromaDB中搜索相似内容 | Search similar content in ChromaDB

3. 🤖 AI生成答案 | AI Generate Answer
   - Claude API处理上下文 | Claude API processes context
   - 结合搜索结果生成回答 | Generate answer with search results

4. 📤 返回结果 | Return Result
   - 格式化答案 | Format answer
   - 显示来源引用 | Show source citations
```

### ✨ 3.2 功能添加类 | Adding Features

#### 初学者友好模板 | Beginner-Friendly Templates

**简单功能添加 | Simple Feature Addition**：
```
我想添加一个[功能名称]
要求：
1. [具体需求1]
2. [具体需求2]
请一步步实现，并解释每一步的作用

I want to add [feature name]
Requirements:
1. [specific requirement 1]
2. [specific requirement 2]
Please implement step by step and explain each step
```

#### 高级功能模板 | Advanced Feature Templates

**复杂功能实现 | Complex Feature Implementation**：
```
使用计划模式实现以下功能：
Feature: [功能名称]
技术栈：[技术要求]
性能要求：[性能指标]
请先展示实现计划，确认后再执行

Use planning mode to implement:
Feature: [feature name]
Tech stack: [technical requirements]
Performance: [performance metrics]
Show implementation plan first, execute after confirmation
```

#### 实战案例：添加深色模式 | Case Study: Adding Dark Mode

```markdown
提示 | Prompt:
添加深色/浅色主题切换功能
要求：
1. 右上角放置切换按钮
2. 使用太阳/月亮图标
3. 切换时有平滑过渡动画
4. 保存用户偏好设置

Add dark/light theme toggle
Requirements:
1. Place toggle button in top-right
2. Use sun/moon icons
3. Smooth transition animation
4. Save user preference

Claude实现步骤 | Claude's Implementation Steps:
1. ✅ 创建CSS变量系统 | Create CSS variable system
2. ✅ 添加主题切换按钮 | Add theme toggle button
3. ✅ 实现JavaScript逻辑 | Implement JavaScript logic
4. ✅ 添加localStorage存储 | Add localStorage storage
5. ✅ 测试各种主题下的显示效果 | Test display in both themes
```

### 🐛 3.3 调试修复类 | Debug & Fix

#### 错误调试模板 | Error Debugging Templates

**基础调试 | Basic Debugging**：
```
我遇到了这个错误：[错误信息]
请帮我：
1. 解释错误原因
2. 提供解决方案
3. 解释如何避免类似错误

I encountered this error: [error message]
Please help me:
1. Explain the cause
2. Provide solution
3. Explain how to avoid similar errors
```

**深度调试 | Deep Debugging**：
```
使用extended thinking模式调试这个复杂问题：
[问题描述]
think hard

Use extended thinking mode to debug this complex issue:
[problem description]
think hard
```

#### 实战案例：修复API错误 | Case Study: Fix API Error

```markdown
场景 | Scenario:
RAG聊天机器人返回"query failed"错误
RAG chatbot returns "query failed" error

调试提示 | Debug Prompt:
聊天机器人对所有问题都返回"query failed"
请：
1. 写测试找出问题所在
2. 定位具体错误代码
3. 修复并验证

Chatbot returns "query failed" for all questions
Please:
1. Write tests to find the issue
2. Locate specific error code
3. Fix and verify

Claude的调试过程 | Claude's Debug Process:
1. 📝 创建测试文件 | Create test files
   - 测试API端点 | Test API endpoints
   - 测试搜索功能 | Test search function
   
2. 🔍 定位问题 | Locate issue
   - 发现MAX_RESULTS设置为0 | Found MAX_RESULTS set to 0
   
3. ✅ 修复问题 | Fix issue
   - 修改配置文件 | Modify config file
   - 重新运行测试 | Rerun tests
```

### 🔄 3.4 代码重构类 | Code Refactoring

#### 重构模板 | Refactoring Templates

**性能优化 | Performance Optimization**：
```
分析 @文件名 的性能瓶颈并优化
要求：
- 保持功能不变
- 提高执行效率
- 添加性能测试

Analyze @filename performance bottlenecks and optimize
Requirements:
- Keep functionality unchanged
- Improve execution efficiency  
- Add performance tests
```

**代码质量提升 | Code Quality Improvement**：
```
重构这个代码使其更易维护：
1. 提取重复代码为函数
2. 改善命名规范
3. 添加类型注解
4. 编写单元测试

Refactor this code for better maintainability:
1. Extract duplicate code into functions
2. Improve naming conventions
3. Add type annotations
4. Write unit tests
```

---

## 第4章：高级功能 | Chapter 4: Advanced Features

### 🧠 4.1 Extended Thinking 深度思考模式 | Extended Thinking Mode

**什么是深度思考？| What is Extended Thinking?**

> 💡 **初学者理解**：就像让Claude"深呼吸，慢慢想"，用更多时间思考复杂问题
> 
> **Beginner's Understanding**: Like asking Claude to "take a deep breath and think slowly", using more time for complex problems

> 🎯 **专业解释**：分配更多计算资源进行多步推理和深度分析
> 
> **Professional Explanation**: Allocating more computational resources for multi-step reasoning and deep analysis

**思考级别 | Thinking Levels**：

| 级别 | Level | 命令 | Command | 适用场景 | Use Case |
|------|-------|------|---------|----------|----------|
| 1️⃣ 基础 | Basic | `think` | 中等复杂问题 | Medium complexity |
| 2️⃣ 深度 | Deep | `think hard` | 复杂算法设计 | Complex algorithm design |
| 3️⃣ 极深 | Very Deep | `think harder` | 架构级决策 | Architecture decisions |
| 4️⃣ 终极 | Ultimate | `ultrathink` | 极其复杂的问题 | Extremely complex problems |

**使用示例 | Usage Example**：

```markdown
你 | You: 
设计一个高性能的分布式缓存系统，需要考虑一致性、可用性和分区容错性
think hard

Design a high-performance distributed cache system considering consistency, availability, and partition tolerance
think hard

Claude: [进入深度思考模式 | Entering deep thinking mode...]
        
        让我深入分析这个问题... | Let me analyze this deeply...
        
        1. CAP定理权衡 | CAP theorem trade-offs
        2. 一致性哈希设计 | Consistent hashing design
        3. 故障转移机制 | Failover mechanisms
        4. 数据复制策略 | Data replication strategies
        [详细的架构设计... | Detailed architecture design...]
```

### 🤖 4.2 Subagents 子代理系统 | Subagent System

**概念理解 | Concept Understanding**：

> 💡 **初学者理解**：就像Claude可以"分身"，同时处理多个任务
> 
> **Beginner's Understanding**: Like Claude can "clone itself" to handle multiple tasks simultaneously

> 🎯 **专业解释**：并行任务处理系统，每个子代理有独立的上下文和专门功能
> 
> **Professional Explanation**: Parallel task processing system, each subagent has independent context and specialized functions

**使用场景 | Use Cases**：

1. **并行调试 | Parallel Debugging**
   ```
   使用两个subagents同时调试前端和后端问题
   Use two subagents to debug frontend and backend issues simultaneously
   ```

2. **多方案探索 | Multi-Solution Exploration**
   ```
   让三个subagents分别用不同方法解决同一问题，然后比较结果
   Have three subagents solve the same problem with different approaches, then compare
   ```

**实战示例 | Practical Example**：

```markdown
你 | You:
使用两个并行subagents来重构这个项目：
- Agent 1: 优化后端API性能
- Agent 2: 改进前端用户体验
最后整合两者的改进

Use two parallel subagents to refactor this project:
- Agent 1: Optimize backend API performance  
- Agent 2: Improve frontend user experience
Finally integrate both improvements

Claude: 启动并行子代理... | Launching parallel subagents...

[Agent 1 工作中 | Agent 1 working...]
- 分析API瓶颈 | Analyzing API bottlenecks
- 实施缓存策略 | Implementing caching strategy
- 优化数据库查询 | Optimizing database queries

[Agent 2 工作中 | Agent 2 working...]
- 改进加载动画 | Improving loading animations
- 优化响应式设计 | Optimizing responsive design
- 添加用户反馈 | Adding user feedback

[整合结果 | Integrating results...]
```

### 🔌 4.3 MCP服务器集成 | MCP Server Integration

**什么是MCP？| What is MCP?**

> 💡 **初学者理解**：像给Claude安装"插件"，让它能使用外部工具
> 
> **Beginner's Understanding**: Like installing "plugins" for Claude to use external tools

> 🎯 **专业定义**：Model Context Protocol，标准化的工具集成协议
> 
> **Professional Definition**: Model Context Protocol, standardized tool integration protocol

#### 常用MCP服务器 | Common MCP Servers

**1. Playwright - 浏览器自动化 | Browser Automation**

安装 | Installation:
```bash
claude mcp add playwright npx @playwright/mcp@latest
```

使用示例 | Usage Example:
```markdown
你 | You: 
使用playwright访问我的网站localhost:3000，截图并检查是否响应式

Use playwright to visit my website localhost:3000, take screenshot and check if responsive

Claude: 我将使用Playwright MCP服务器来测试您的网站...
        I'll use Playwright MCP server to test your website...
        
        1. 打开浏览器 | Opening browser
        2. 访问localhost:3000 | Visiting localhost:3000
        3. 截取桌面版截图 | Taking desktop screenshot
        4. 调整为移动设备尺寸 | Resizing to mobile dimensions
        5. 截取移动版截图 | Taking mobile screenshot
        
        [显示截图和分析结果 | Shows screenshots and analysis]
```

**2. Figma - 设计导入 | Design Import**

安装 | Installation:
```bash
# 官方版（需要Pro账号）| Official (needs Pro account)
claude mcp add --transport http figma-dev-mode-mcp-server http://127.0.0.1:3845/mcp

# 免费替代版 | Free alternative
claude mcp add "Framelink-Figma" npx -y figma-developer-mcp --figma-api-key=YOUR-KEY --stdio
```

使用示例 | Usage Example:
```markdown
你 | You:
使用Figma MCP分析这个设计稿[链接]，并创建对应的React组件

Use Figma MCP to analyze this design [link] and create corresponding React components

Claude: 正在连接Figma获取设计信息...
        Connecting to Figma to fetch design information...
        
        分析到以下组件 | Found following components:
        - Header导航栏 | Header navigation
        - Hero区域 | Hero section
        - 特性卡片 | Feature cards
        
        [生成React代码 | Generating React code...]
```

### 🌳 4.4 Git Worktrees 并行开发 | Parallel Development

**概念理解 | Concept Understanding**：

> 💡 **初学者理解**：像同时打开同一个项目的多个"副本"，每个副本开发不同功能
> 
> **Beginner's Understanding**: Like opening multiple "copies" of the same project, each developing different features

> 🎯 **专业解释**：Git的工作树功能，允许同一仓库的多个工作目录并行开发
> 
> **Professional Explanation**: Git's worktree feature, allowing multiple working directories of the same repository for parallel development

**使用流程 | Usage Flow**：

```bash
# 1. 创建worktree目录 | Create worktree directory
mkdir .trees

# 2. 为每个功能创建worktree | Create worktree for each feature
git worktree add .trees/feature-auth      # 认证功能 | Auth feature
git worktree add .trees/feature-payment   # 支付功能 | Payment feature
git worktree add .trees/feature-ui        # UI改进 | UI improvements

# 3. 在每个worktree中启动Claude | Launch Claude in each worktree
cd .trees/feature-auth && claude
cd .trees/feature-payment && claude
cd .trees/feature-ui && claude

# 4. 合并所有改进 | Merge all improvements
git merge .trees/feature-auth/main
git merge .trees/feature-payment/main
git merge .trees/feature-ui/main
```

**实战案例 | Practical Case**：

```markdown
场景：同时开发三个功能 | Scenario: Develop three features simultaneously

功能1 - 深色模式 | Feature 1 - Dark Mode:
你：在.trees/dark-mode中添加深色模式切换
You: Add dark mode toggle in .trees/dark-mode

功能2 - 用户认证 | Feature 2 - User Auth:
你：在.trees/user-auth中实现JWT认证
You: Implement JWT authentication in .trees/user-auth

功能3 - 数据可视化 | Feature 3 - Data Visualization:
你：在.trees/data-viz中添加图表功能
You: Add chart functionality in .trees/data-viz

最终：Claude自动合并所有功能，解决冲突
Finally: Claude auto-merges all features, resolves conflicts
```

### 🎣 4.5 Hooks 钩子系统 | Hooks System

**概念理解 | Concept Understanding**：

> 💡 **初学者理解**：像设置"触发器"，当Claude执行特定操作时自动运行你的脚本
> 
> **Beginner's Understanding**: Like setting "triggers" that auto-run your scripts when Claude performs specific actions

> 🎯 **专业定义**：生命周期钩子，在Claude Code特定事件时执行自定义Shell命令
> 
> **Professional Definition**: Lifecycle hooks that execute custom shell commands at specific Claude Code events

**钩子类型 | Hook Types**：

| 钩子 | Hook | 触发时机 | Trigger | 用途 | Use Case |
|------|------|---------|---------|------|----------|
| `before-tool` | 工具执行前 | Before tool execution | 验证、备份 | Validation, backup |
| `after-tool` | 工具执行后 | After tool execution | 清理、通知 | Cleanup, notification |
| `subagent-complete` | 子代理完成 | Subagent completion | 结果处理 | Result processing |
| `claude-complete` | Claude完成 | Claude completion | 最终检查 | Final checks |

**配置示例 | Configuration Example**：

在 `.claude/hooks.json` 中配置 | Configure in `.claude/hooks.json`:

```json
{
  "hooks": {
    "before-tool": {
      "command": "echo '工具执行前备份' && git stash",
      "description": "在执行工具前自动备份"
    },
    "after-tool": {
      "command": "npm test",
      "description": "工具执行后自动运行测试"
    }
  }
}
```

---

## 第5章：项目实战案例 | Chapter 5: Real Projects

### 💬 5.1 RAG聊天机器人项目 | RAG Chatbot Project

**项目目标 | Project Goal**：
创建一个智能问答系统，能够基于文档库回答用户问题。
Create an intelligent Q&A system that answers user questions based on document library.

#### Phase 1: 项目初始化 | Project Initialization

```markdown
步骤1：创建项目结构 | Step 1: Create project structure

你 | You: 
创建一个RAG聊天机器人项目，包含前后端分离架构
使用Python FastAPI后端和HTML/JS前端

Create a RAG chatbot project with frontend-backend separation
Use Python FastAPI backend and HTML/JS frontend

Claude生成的结构 | Claude generates structure:
rag-chatbot/
├── backend/
│   ├── app.py              # FastAPI主应用 | Main FastAPI app
│   ├── rag_system.py       # RAG核心逻辑 | RAG core logic
│   ├── vector_store.py     # 向量数据库 | Vector database
│   ├── ai_generator.py     # AI生成器 | AI generator
│   └── search_tools.py     # 搜索工具 | Search tools
├── frontend/
│   ├── index.html          # 主页面 | Main page
│   ├── style.css           # 样式 | Styles
│   └── script.js           # 交互逻辑 | Interaction logic
└── docs/                   # 文档目录 | Document directory
```

#### Phase 2: 核心功能实现 | Core Feature Implementation

```markdown
步骤2：实现文档处理 | Step 2: Implement document processing

你 | You:
实现文档处理功能：
1. 读取docs文件夹中的文档
2. 分割成合适大小的chunks
3. 生成向量embeddings
4. 存储到ChromaDB

Implement document processing:
1. Read documents from docs folder
2. Split into appropriate chunks  
3. Generate vector embeddings
4. Store in ChromaDB

Claude的实现要点 | Claude's implementation points:
- 智能分句，保持语义完整 | Smart sentence splitting
- 800字符chunks，100字符重叠 | 800 char chunks, 100 char overlap
- 使用sentence-transformers生成向量 | Use sentence-transformers
- 双集合策略：metadata + content | Dual collection strategy
```

#### Phase 3: 功能增强 | Feature Enhancement

```markdown
步骤3：添加高级功能 | Step 3: Add advanced features

功能1：嵌入链接 | Feature 1: Embed links
你：为每个引用的来源添加可点击链接
You: Add clickable links for each cited source

功能2：新建对话 | Feature 2: New chat
你：添加"+ NEW CHAT"按钮清空对话
You: Add "+ NEW CHAT" button to clear conversation

功能3：多工具支持 | Feature 3: Multi-tool support
你：让AI可以连续调用多个搜索工具
You: Allow AI to call multiple search tools sequentially
```

#### 完整实现流程图 | Complete Implementation Flow

```
用户输入 User Input
    ↓
前端处理 Frontend Processing
    ↓
API请求 API Request (/api/query)
    ↓
RAG系统 RAG System
    ├── 会话管理 Session Management
    ├── 向量搜索 Vector Search
    └── AI生成 AI Generation
    ↓
返回结果 Return Result
    ↓
前端展示 Frontend Display
```

### 📊 5.2 数据分析Dashboard项目 | Data Analysis Dashboard Project

**项目目标 | Project Goal**：
将Jupyter Notebook的探索性分析转换为交互式Dashboard。
Convert Jupyter Notebook exploratory analysis into interactive dashboard.

#### Phase 1: Notebook重构 | Notebook Refactoring

```markdown
原始状态 | Original State:
- 混乱的EDA.ipynb | Messy EDA.ipynb
- 硬编码的2023年数据 | Hardcoded 2023 data
- 重复的代码片段 | Duplicate code snippets

重构目标 | Refactoring Goals:
1. 模块化代码结构 | Modular code structure
2. 可配置的时间范围 | Configurable time range
3. 可重用的业务逻辑 | Reusable business logic

提示 | Prompt:
重构@EDA.ipynb，要求：
1. 创建data_loader.py处理数据加载
2. 创建business_metrics.py计算业务指标
3. 使分析可配置（年份、月份）
4. 保持相同的分析和图表

Refactor @EDA.ipynb, requirements:
1. Create data_loader.py for data loading
2. Create business_metrics.py for business metrics
3. Make analysis configurable (year, month)
4. Keep same analysis and charts
```

#### Phase 2: Dashboard创建 | Dashboard Creation

```markdown
Dashboard布局设计 | Dashboard Layout Design:

┌─────────────────────────────────────┐
│     标题          [年份选择器]        │
│     Title         [Year Selector]    │
├─────────────────────────────────────┤
│  KPI卡片 | KPI Cards (4 columns)    │
│  收入 | 增长 | 订单值 | 订单数        │
│  Revenue|Growth|Order Value|Orders   │
├──────────────┬──────────────────────┤
│ 收入趋势图    │  产品类别排名         │
│ Revenue Trend │  Category Ranking    │
├──────────────┼──────────────────────┤
│ 地理分布图    │  满意度分析           │
│ Geo Map      │  Satisfaction        │
├──────────────┴──────────────────────┤
│ 配送时间 | 评分  (底部指标)           │
│ Delivery | Score (Bottom metrics)    │
└─────────────────────────────────────┘

实现提示 | Implementation Prompt:
将@EDA_Refactored.ipynb转换为Streamlit dashboard
要求：
1. 使用上述布局
2. 全局年份筛选器
3. 使用Plotly创建交互式图表
4. KPI卡片显示趋势箭头

Convert @EDA_Refactored.ipynb to Streamlit dashboard
Requirements:
1. Use above layout
2. Global year filter
3. Use Plotly for interactive charts
4. KPI cards show trend arrows
```

#### Phase 3: 功能优化 | Feature Optimization

```python
# 关键代码片段 | Key Code Snippets

# 1. 数据缓存优化 | Data caching optimization
@st.cache_data
def load_data(year):
    """缓存数据加载，避免重复读取
    Cache data loading to avoid repeated reads"""
    loader = EcommerceDataLoader()
    return loader.load_year_data(year)

# 2. KPI计算 | KPI calculation
def calculate_kpis(data, previous_data):
    """计算关键业务指标和趋势
    Calculate key business metrics and trends"""
    return {
        'revenue': data['price'].sum(),
        'growth': calculate_growth(data, previous_data),
        'aov': data['price'].mean(),
        'orders': data['order_id'].nunique()
    }

# 3. 响应式布局 | Responsive layout
col1, col2, col3, col4 = st.columns(4)
with col1:
    display_metric("Revenue", revenue, trend)
```

### 🎨 5.3 Figma设计转代码项目 | Figma to Code Project

**项目目标 | Project Goal**：
将Figma设计稿自动转换为可运行的Web应用。
Automatically convert Figma design to runnable web application.

#### Phase 1: 环境准备 | Environment Setup

```bash
# 1. 初始化Next.js项目 | Initialize Next.js project
npx create-next-app@latest my-dashboard --typescript --tailwind

# 2. 配置Figma MCP | Configure Figma MCP
claude mcp add figma-dev npx -y figma-developer-mcp --figma-api-key=YOUR-KEY --stdio

# 3. 配置Playwright MCP（用于预览）| Configure Playwright MCP (for preview)
claude mcp add playwright npx @playwright/mcp@latest
```

#### Phase 2: 设计导入与实现 | Design Import & Implementation

```markdown
提示模板 | Prompt Template:

使用Figma MCP分析这个设计[Figma链接]，然后：
1. 提取所有组件和样式
2. 创建对应的React组件
3. 使用Tailwind CSS实现样式
4. 确保响应式设计
5. 使用Playwright预览并验证

Use Figma MCP to analyze this design [Figma link], then:
1. Extract all components and styles
2. Create corresponding React components
3. Implement styles with Tailwind CSS
4. Ensure responsive design
5. Preview and verify with Playwright

Claude的工作流程 | Claude's workflow:
1. 🎨 连接Figma获取设计数据 | Connect Figma to get design data
2. 📐 分析布局和组件结构 | Analyze layout and component structure
3. 🎯 生成组件代码 | Generate component code
4. 🎨 应用样式和动画 | Apply styles and animations
5. 📱 测试响应式效果 | Test responsive effects
```

#### Phase 3: 数据集成 | Data Integration

```markdown
连接真实数据 | Connect Real Data:

你：将这些图表连接到FRED经济数据API
You: Connect these charts to FRED economic data API

实现步骤 | Implementation steps:
1. 申请FRED API密钥 | Apply for FRED API key
2. 创建数据获取服务 | Create data fetching service
3. 集成到React组件 | Integrate with React components
4. 添加实时更新 | Add real-time updates
```

---

## 第6章：常见问题解答 | Chapter 6: FAQ

### 🔰 6.1 初学者问题 | Beginner Questions

#### Q1: 我完全不会编程，能用Claude Code吗？
#### Can I use Claude Code without any programming knowledge?

**答案 | Answer**: ✅ **完全可以！| Absolutely!**

Claude Code的设计理念就是让编程变得简单：
- 🗣️ 使用自然语言交流 | Communicate in natural language
- 📚 自动生成代码并解释 | Auto-generate and explain code
- 🎓 边用边学，逐步提升 | Learn while using, gradual improvement

**新手建议 | Beginner Tips**：
1. 从简单项目开始（如个人主页）| Start with simple projects (like personal homepage)
2. 让Claude解释每行代码 | Ask Claude to explain each line
3. 逐步尝试修改生成的代码 | Gradually try modifying generated code

#### Q2: Claude Code和ChatGPT有什么区别？
#### What's the difference between Claude Code and ChatGPT?

**主要区别 | Main Differences**：

| 方面 | Aspect | Claude Code | ChatGPT |
|------|--------|------------|---------|
| 专注领域 | Focus | 专门针对编程 | 通用对话 |
| 文件操作 | File Operations | ✅ 直接创建/编辑文件 | ❌ 只能显示代码 |
| 项目理解 | Project Understanding | ✅ 扫描整个代码库 | ❌ 需要手动提供 |
| 工具集成 | Tool Integration | ✅ MCP服务器支持 | ⚠️ 有限的插件 |
| 执行模式 | Execution Mode | ✅ 可直接执行命令 | ❌ 只能提供指导 |

#### Q3: 什么时候该用think命令？
#### When should I use the think command?

**使用指南 | Usage Guide**：

- **不需要think | No need for think**：
  - ✅ 简单的CRUD操作 | Simple CRUD operations
  - ✅ 基础UI调整 | Basic UI adjustments
  - ✅ 常见bug修复 | Common bug fixes

- **需要think | Need think**：
  - 🤔 算法优化 | Algorithm optimization
  - 🤔 架构设计 | Architecture design
  - 🤔 性能调优 | Performance tuning

- **需要think hard | Need think hard**：
  - 🧠 分布式系统设计 | Distributed system design
  - 🧠 复杂的并发问题 | Complex concurrency issues
  - 🧠 安全漏洞分析 | Security vulnerability analysis

### 💻 6.2 技术问题 | Technical Questions

#### Q4: 如何处理"token limit exceeded"错误？
#### How to handle "token limit exceeded" error?

**解决方案 | Solutions**：

1. **使用/compact压缩对话 | Use /compact to compress conversation**
   ```
   /compact
   # 保留关键信息，清理冗余内容
   # Keep key info, clean redundant content
   ```

2. **使用/clear重新开始 | Use /clear to restart**
   ```
   /clear
   # 完全清空，适合新任务
   # Complete clear, suitable for new tasks
   ```

3. **优化提示词 | Optimize prompts**
   - ❌ 避免："给我看所有代码" | Avoid: "Show me all code"
   - ✅ 推荐："修改登录函数" | Recommend: "Modify login function"

#### Q5: MCP服务器连接失败怎么办？
#### What to do when MCP server connection fails?

**排查步骤 | Troubleshooting Steps**：

1. **检查MCP状态 | Check MCP status**
   ```
   /mcp
   # 查看已连接的服务器
   # View connected servers
   ```

2. **重新添加服务器 | Re-add server**
   ```bash
   # 先退出Claude Code
   exit
   
   # 重新添加MCP
   claude mcp add [server-name] [command]
   
   # 重新启动
   claude
   ```

3. **检查依赖 | Check dependencies**
   - Node.js版本 ≥ 18 | Node.js version ≥ 18
   - NPM正确安装 | NPM properly installed
   - 网络连接正常 | Network connection normal

#### Q6: 如何优化Claude Code的响应速度？
#### How to optimize Claude Code response speed?

**优化技巧 | Optimization Tips**：

1. **精确指定文件 | Specify files precisely**
   ```
   # ❌ 慢：扫描整个项目
   # Slow: Scan entire project
   "优化项目性能"
   
   # ✅ 快：指定具体文件
   # Fast: Specify exact files
   "优化@api/user.js的查询性能"
   ```

2. **使用项目记忆 | Use project memory**
   ```
   /init  # 首次创建CLAUDE.md
   #添加常用信息到记忆
   ```

3. **合理使用模式 | Use modes wisely**
   - 简单任务：自动执行模式 | Simple tasks: Auto-execute
   - 复杂任务：计划模式 | Complex tasks: Planning mode

### 🚀 6.3 最佳实践问题 | Best Practice Questions

#### Q7: 如何写出更好的prompts？
#### How to write better prompts?

**Prompt优化原则 | Prompt Optimization Principles**：

**1. 明确具体 | Be Specific**
```markdown
❌ 模糊 | Vague:
"改进代码"
"Improve code"

✅ 具体 | Specific:
"重构@utils/api.js，提取重复的错误处理逻辑为独立函数"
"Refactor @utils/api.js, extract duplicate error handling into separate function"
```

**2. 提供上下文 | Provide Context**
```markdown
❌ 缺少上下文 | Lacking context:
"添加缓存"
"Add cache"

✅ 包含上下文 | With context:
"在@api/products.js的getProducts函数添加Redis缓存，TTL设为5分钟"
"Add Redis cache to getProducts function in @api/products.js, TTL 5 minutes"
```

**3. 分步骤描述 | Step-by-step Description**
```markdown
✅ 好的模板 | Good template:
"请帮我实现用户认证功能：
1. 创建JWT token生成函数
2. 实现登录API端点
3. 添加认证中间件
4. 创建前端登录表单
请逐步实现并解释"

"Help me implement user authentication:
1. Create JWT token generation function
2. Implement login API endpoint
3. Add authentication middleware
4. Create frontend login form
Please implement step by step with explanations"
```

#### Q8: 如何有效管理大型项目？
#### How to manage large projects effectively?

**项目管理策略 | Project Management Strategies**：

1. **模块化开发 | Modular Development**
   ```
   项目结构 | Project structure:
   /src
     /modules
       /auth      # 认证模块 | Auth module
       /payment   # 支付模块 | Payment module
       /user      # 用户模块 | User module
   
   # 每个模块独立开发和测试
   # Develop and test each module independently
   ```

2. **使用Git Worktrees并行开发 | Use Git Worktrees for parallel development**
   ```bash
   # 为每个功能创建worktree
   # Create worktree for each feature
   git worktree add .trees/feature-x
   git worktree add .trees/feature-y
   ```

3. **维护CLAUDE.md | Maintain CLAUDE.md**
   ```markdown
   # 定期更新项目信息
   # Regularly update project info
   /init  # 重新扫描
   #项目使用PostgreSQL数据库
   #API需要JWT认证
   #前端使用React 18
   ```

#### Q9: 如何确保生成代码的质量？
#### How to ensure generated code quality?

**质量保证方法 | Quality Assurance Methods**：

1. **要求测试 | Request Tests**
   ```
   "实现功能后，请同时编写单元测试"
   "After implementing, please write unit tests"
   ```

2. **代码审查 | Code Review**
   ```
   "请review这段代码，指出潜在问题"
   "Please review this code and point out potential issues"
   ```

3. **性能检查 | Performance Check**
   ```
   "分析这个函数的时间复杂度，并优化"
   "Analyze time complexity of this function and optimize"
   ```

---

## 附录：专业术语词汇表 | Appendix: Glossary

### 🔤 编程基础术语 | Programming Basics

| 中文 | English | 初学者解释 | 专业定义 |
|------|---------|-----------|---------|
| 变量 | Variable | 存储数据的容器，像贴了标签的盒子 | 程序中用于存储数据的命名内存位置 |
| 函数 | Function | 完成特定任务的代码块，像工具箱中的工具 | 可重用的代码单元，接受输入并返回输出 |
| 类 | Class | 创建对象的模板，像建筑图纸 | 面向对象编程中定义对象属性和方法的蓝图 |
| API | API | 程序之间的沟通桥梁 | Application Programming Interface，定义软件组件交互的接口 |
| 数据库 | Database | 组织化存储数据的仓库 | 结构化数据的持久化存储系统 |
| 前端 | Frontend | 用户看到和交互的界面 | 应用程序的客户端，负责用户界面和交互 |
| 后端 | Backend | 处理业务逻辑的服务器端 | 应用程序的服务器端，处理数据和业务逻辑 |
| 框架 | Framework | 预设好的程序骨架 | 提供应用程序基础结构的软件平台 |
| 调试 | Debug | 找出并修复程序错误 | 识别和修复软件缺陷的过程 |
| 重构 | Refactor | 改进代码结构但不改变功能 | 在不改变外部行为的情况下改进代码内部结构 |

### 🤖 AI/LLM相关术语 | AI/LLM Terms

| 术语 | Term | 解释 | Explanation |
|------|------|------|-------------|
| LLM | Large Language Model | 大语言模型，能理解和生成人类语言的AI | AI trained on vast text data to understand and generate human language |
| Token | Token | AI处理文本的基本单位，类似"字" | Basic unit of text processing in AI, similar to words or subwords |
| Embedding | 向量嵌入 | 将文本转换为数字向量的技术 | Technique to convert text into numerical vectors |
| RAG | Retrieval-Augmented Generation | 检索增强生成，先搜索再回答 | Combining retrieval with generation for better answers |
| Prompt | 提示词 | 给AI的指令或问题 | Instructions or questions given to AI |
| Context | 上下文 | AI理解问题时参考的背景信息 | Background information AI uses to understand queries |
| Fine-tuning | 微调 | 针对特定任务训练模型 | Training a model for specific tasks |

### 🛠️ Claude Code专有术语 | Claude Code Specific Terms

| 术语 | Term | 用途 | Usage | 示例 | Example |
|------|------|------|-------|------|---------|
| `/init` | 初始化 | 扫描项目创建CLAUDE.md | Scan project and create CLAUDE.md | `/init` |
| `/clear` | 清空 | 清除对话历史 | Clear conversation history | `/clear` |
| `/compact` | 压缩 | 压缩对话保留关键信息 | Compress conversation keeping key info | `/compact` |
| `#` | 记忆 | 添加项目特定信息 | Add project-specific information | `#使用TypeScript` |
| `@` | 引用 | 引用特定文件 | Reference specific files | `@src/index.js` |
| Extended Thinking | 深度思考 | 处理复杂问题 | Handle complex problems | `think hard` |
| Subagent | 子代理 | 并行处理任务 | Parallel task processing | `使用subagent调试` |
| MCP | Model Context Protocol | 连接外部工具 | Connect external tools | `/mcp` |
| Worktree | 工作树 | Git并行开发 | Git parallel development | `git worktree add` |
| Hook | 钩子 | 自动执行脚本 | Auto-execute scripts | `before-tool hook` |

### 🌐 Web开发术语 | Web Development Terms

| 术语 | Term | 解释 | Explanation |
|------|------|------|-------------|
| HTML | HyperText Markup Language | 网页结构语言 | Language for web page structure |
| CSS | Cascading Style Sheets | 网页样式语言 | Language for web page styling |
| JavaScript | JS | 网页交互编程语言 | Programming language for web interactivity |
| React | React | Facebook开发的前端框架 | Frontend framework by Facebook |
| FastAPI | FastAPI | Python的现代Web框架 | Modern Python web framework |
| REST API | RESTful API | 网络服务接口标准 | Web service interface standard |
| JSON | JavaScript Object Notation | 数据交换格式 | Data interchange format |
| CORS | Cross-Origin Resource Sharing | 跨域资源共享 | Mechanism for cross-domain requests |
| JWT | JSON Web Token | 身份认证令牌 | Authentication token format |
| WebSocket | WebSocket | 实时双向通信协议 | Real-time bidirectional communication protocol |

### 📊 数据处理术语 | Data Processing Terms

| 术语 | Term | 解释 | Explanation |
|------|------|------|-------------|
| DataFrame | 数据框 | 表格形式的数据结构 | Tabular data structure |
| SQL | Structured Query Language | 数据库查询语言 | Database query language |
| NoSQL | 非关系型数据库 | 灵活的数据存储方式 | Flexible data storage approach |
| ETL | Extract, Transform, Load | 数据处理流程 | Data processing pipeline |
| Vector Database | 向量数据库 | 存储和搜索向量的数据库 | Database for storing and searching vectors |
| ChromaDB | ChromaDB | 开源向量数据库 | Open-source vector database |
| Pandas | Pandas | Python数据分析库 | Python data analysis library |
| NumPy | NumPy | Python数值计算库 | Python numerical computing library |

---

## 🎯 总结 | Summary

### 核心要点回顾 | Key Points Review

1. **Claude Code是什么 | What is Claude Code**
   - 🤖 AI编程助手，理解自然语言
   - 📝 直接操作文件，不只是显示代码
   - 🔧 集成多种工具，扩展能力强

2. **适合谁使用 | Who Should Use It**
   - 🔰 编程初学者：降低入门门槛
   - 💼 专业开发者：提高开发效率
   - 📊 数据分析师：快速处理数据

3. **如何用好它 | How to Use It Well**
   - ✍️ 清晰具体的提示词
   - 📁 良好的项目组织
   - 🔄 持续的反馈优化

### 学习路径建议 | Learning Path Suggestions

**初学者路线 | Beginner Path**:
1. 第1周：基础命令和简单项目
2. 第2周：尝试修改生成的代码
3. 第3周：独立完成小项目
4. 第4周：学习高级功能

**进阶路线 | Advanced Path**:
1. 掌握Extended Thinking
2. 学习Subagents并行开发
3. 集成MCP服务器
4. 自定义Hooks和工作流

### 持续学习资源 | Continuous Learning Resources

- 📚 [官方文档 | Official Docs](https://docs.anthropic.com/en/docs/claude-code)
- 🎓 [Anthropic Academy课程 | Anthropic Academy](https://anthropic.skilljar.com/claude-code-in-action)
- 💡 [最佳实践 | Best Practices](https://www.anthropic.com/engineering/claude-code-best-practices)
- 🌟 [使用案例 | Use Cases](https://www.anthropic.com/news/how-anthropic-teams-use-claude-code)

---

## 📮 反馈与支持 | Feedback & Support

**遇到问题？| Having Issues?**
- 使用 `/help` 命令获取帮助
- 访问 [GitHub Issues](https://github.com/anthropics/claude-code/issues) 报告问题

**想要贡献？| Want to Contribute?**
- 分享你的使用经验
- 提供更好的prompt模板
- 参与社区讨论

---

> 💡 **最后一句话 | Final Words**：
> 
> Claude Code不仅是工具，更是你的编程伙伴。无论你是刚开始编程之旅，还是已经是经验丰富的开发者，它都能帮助你更高效、更愉快地创造。
> 
> Claude Code is not just a tool, but your programming partner. Whether you're just starting your coding journey or you're an experienced developer, it helps you create more efficiently and enjoyably.

**祝编程愉快！| Happy Coding! 🚀**
# 🚀 Claude Code Advanced Configuration Reference

> **A comprehensive collection of production-grade Claude Code configurations, specialized agents, and automation workflows for optimizing AI-assisted development**

## 📚 Purpose

This repository serves as an **educational reference** for developers looking to maximize their productivity with Claude Code. It demonstrates advanced configuration patterns, custom agents, and automation workflows that have been refined through extensive real-world usage in building production AI systems, MCP servers, and vector databases.

**⚠️ Note:** This is a reference repository intended for learning. All credentials shown are placeholders. Adapt these patterns to your specific needs and environment.

## 🎯 What You'll Learn

- **🤖 Create specialized AI agents** for domain-specific expertise
- **⚙️ Configure advanced permissions** and security controls  
- **🔧 Build custom commands** for complex workflows
- **🚀 Automate repetitive tasks** with intelligent hooks
- **💾 Implement memory systems** with vector search
- **🏗️ Deploy production MCP servers** with monitoring
- **🔍 Debug and optimize** AI-assisted development

## 📁 Repository Structure

```text
memory-mcp-server/     # MCP server with memory & vector search
├── .claude/
│   ├── agents/        # 15 specialized AI agents
│   ├── commands/      # 7 custom workflow commands
│   ├── hooks/         # 2 automation scripts
│   └── settings.json  # Central configuration
├── CLAUDE.md          # MCP development guide
└── README.md          # Setup documentation

nextjs-15/             # Complete Next.js 15 configuration
├── .claude/
│   ├── agents/        # 11 Next.js-specific agents
│   ├── commands/      # 6 workflow commands
│   ├── hooks/         # Validation & formatting
│   └── settings.json
├── CLAUDE.md          # Next.js 15 best practices
└── README.md          # Setup guide
```

## 🎯 Available Configurations

### Memory MCP Server Configuration

A production-grade configuration for building MCP servers with memory persistence and vector search:

- **15 Specialized Agents** for MCP, database, and memory systems
- **7 Custom Commands** for development workflows
- **2 Automation Hooks** for TypeScript and logging
- **Optimized for:** PostgreSQL 17, pgvector, Drizzle ORM, MCP SDK

[View Memory MCP Server Details →](./memory-mcp-server/README.md)

## 🎯 Framework-Specific Configurations

### Next.js 15 Configuration

A complete Claude Code configuration tailored for Next.js 15 development, including:

#### Specialized Next.js Agents (11 total)

**Core Development:**

- **`nextjs-app-router`** - App Router routing patterns and best practices
- **`nextjs-server-components`** - Server/Client component optimization
- **`nextjs-server-actions`** - Forms, mutations, and progressive enhancement
- **`nextjs-data-fetching`** - Caching strategies and streaming
- **`nextjs-performance`** - Bundle analysis and Core Web Vitals

**Infrastructure & Quality:**

- **`nextjs-testing`** - Jest, Vitest, Playwright setup
- **`nextjs-deployment`** - Docker, Vercel, AWS deployment
- **`nextjs-migration`** - Pages Router to App Router migration
- **`nextjs-security`** - Authentication, CSP, OWASP compliance
- **`nextjs-debugging`** - React DevTools and troubleshooting
- **`nextjs-typescript`** - Type safety and error resolution

#### Next.js Commands (6 total)

```bash
/create-page [route]          # Generate page with loading/error boundaries
/create-server-action [name]  # Create type-safe Server Actions
/optimize-components          # Analyze component boundaries
/setup-testing [framework]    # Configure testing framework
/analyze-performance          # Generate performance report
/migrate-to-app-router        # Migrate from Pages Router
```

#### Key Features

- **React 19 & Async Request APIs** - Full support for Next.js 15 breaking changes
- **Server Components First** - Optimized for minimal client JavaScript
- **Intelligent Validation** - Pre-commit hooks for Next.js patterns
- **Best Practices Enforcement** - Automated checks for common mistakes
- **Complete Documentation** - CLAUDE.md with Next.js 15 patterns

## 🛠️ Featured Commands

### Memory MCP Server Commands

```bash
/setup quick       # Quick MCP project setup
/setup full        # Complete environment with dependencies
/setup database    # PostgreSQL & pgvector initialization
/mcp-debug        # Debug MCP protocol issues
/memory-ops       # Test memory CRUD operations
```

### Next.js 15 Commands

```bash
/create-page              # Generate page with boundaries
/create-server-action     # Create type-safe Server Actions
/optimize-components      # Analyze component boundaries
/analyze-performance      # Generate performance report
/migrate-to-app-router    # Migrate from Pages Router
```

## ⚡ Shared Features

### Automation Hooks

Both configurations include intelligent hooks:

- **TypeScript Development** - Auto type-check, format, lint
- **Command Logging** - Audit trail with timestamps
- **Smart Filtering** - Skip node_modules, build directories
- **Test Automation** - Run tests on file changes

### Security Best Practices

All configurations enforce:

- 🔒 **Whitelist approach** for commands
- 🚫 **Protected sensitive files** (.env, secrets)
- ✅ **Scoped write permissions** by file type
- 🛡️ **Safe git operations** (no force push)
- 🔐 **Input validation** with Zod schemas

## 💡 Use Cases & Examples

### 1. Memory MCP Server Development

Use the memory-mcp-server configuration for:

- Building MCP servers with persistent memory storage
- Implementing vector search with pgvector and OpenAI embeddings
- Creating multi-tenant AI companion systems
- Setting up production PostgreSQL with Neon
- Deploying with Docker and Kubernetes

### 2. Next.js 15 Application Development

Use the nextjs-15 configuration for:

- Setting up new Next.js 15 projects with best practices
- Migrating from Pages Router to App Router
- Implementing Server Components and Server Actions
- Optimizing performance and Core Web Vitals
- Setting up comprehensive testing
- Deploying to Vercel, Docker, or AWS

### 3. Production Deployment Pipeline

Leverage deployment agents for:

- Docker containerization with security hardening
- Kubernetes orchestration with auto-scaling
- Prometheus/Grafana monitoring setup
- Structured logging and distributed tracing

### 3. AI Companion Development

Build multi-tenant companion systems with:

- Isolated memory spaces per user
- Token-based authentication
- Rate limiting and quota management
- Conversation history with vector search

## 🚀 Getting Started

### 1. Choose Your Configuration

```bash
# For MCP server development
cp -r memory-mcp-server/.claude your-project/
cp memory-mcp-server/CLAUDE.md your-project/

# For Next.js 15 development
cp -r nextjs-15/.claude your-project/
cp nextjs-15/CLAUDE.md your-project/
```

### 2. Explore Available Configurations

```bash
# Memory MCP Server configuration
ls -la memory-mcp-server/.claude/
cat memory-mcp-server/README.md

# Next.js 15 configuration
ls -la nextjs-15/.claude/
cat nextjs-15/README.md
```

### 3. Adapt to Your Workflow

1. **Choose a base configuration** that matches your project type
2. **Customize agents** for your specific needs
3. **Configure permissions** based on your security requirements
4. **Set up hooks** for your development workflow
5. **Merge configurations** if working with multiple frameworks

### 3. Key Configuration Patterns

#### Environment Variables (Placeholder Examples)

```json
"env": {
  "DATABASE_URL": "postgresql://user:pass@host/dbname?sslmode=require",
  "OPENAI_API_KEY": "sk-your-openai-api-key-here",
  "MCP_SERVER_PORT": "3000"
}
```

#### Hook Configuration

```json
"hooks": {
  "PostToolUse": [{
    "matcher": "Edit|MultiEdit|Write",
    "hooks": [{
      "type": "command",
      "command": "$CLAUDE_PROJECT_DIR/.claude/hooks/typescript-dev.sh"
    }]
  }]
}
```

## 📊 Configuration Statistics

### Memory MCP Server Configuration

- **15 Specialized Agents** - ~15,000 lines of domain expertise
- **7 Custom Commands** - Full development lifecycle coverage
- **2 Automation Hooks** - TypeScript and logging automation
- **Focus Areas:** MCP protocol, vector search, memory systems, production deployment

### Next.js 15 Configuration

- **11 Next.js Agents** - Framework-specific expertise
- **6 Workflow Commands** - Next.js development automation
- **Intelligent Hooks** - Validation and formatting
- **Focus Areas:** App Router, Server Components, performance, testing

## 🔗 Technology Stack

This configuration is optimized for:

### General Development

- **TypeScript** & Node.js development
- **PostgreSQL 17** with **Neon** serverless
- **Drizzle ORM v0.44.4** for type-safe database access
- **pgvector v0.8.0** for vector similarity search
- **MCP SDK** for protocol implementation
- **Docker** & **Kubernetes** for deployment

### Framework Support

- **Next.js 15** with App Router
- **React 19** with Server Components
- **Tailwind CSS** for styling
- **Server Actions** for mutations
- **Turbopack** for faster builds

## 📈 Benefits of This Configuration

1. **🚀 10x Faster Development** - Specialized agents handle complex tasks
2. **🛡️ Enhanced Security** - Multi-layered permission controls
3. **🤖 Automated Workflows** - Hooks handle routine tasks
4. **📚 Built-in Expertise** - Deep domain knowledge in agents
5. **🔧 Production-Ready** - Deployment and monitoring included
6. **🧪 Quality Assurance** - Automated testing and review

## 🤝 Contributing

While this is primarily a reference repository, suggestions for improvements are welcome. Consider:

- Additional agent specializations
- New workflow commands
- Enhanced automation hooks
- Security improvements

## 📝 License

This configuration reference is provided as-is for educational purposes. Adapt and modify for your specific needs.

## ⚠️ Important Notes

1. **Reference Only** - This repository is for learning, not direct cloning
2. **Placeholder Values** - All credentials are examples only
3. **Customize for Your Needs** - Adapt patterns to your specific workflow
4. **Security First** - Always review and adjust permissions for your environment

## 🎓 Learning Path

1. **Start Simple** - Begin with `settings.json` permissions
2. **Add Commands** - Implement one custom command
3. **Integrate Agents** - Add relevant specialized agents
4. **Automate** - Set up hooks for your workflow
5. **Iterate** - Refine based on your experience

---

**Built with ❤️ for the Claude Code community**

*Transform your AI-assisted development with production-grade configurations*

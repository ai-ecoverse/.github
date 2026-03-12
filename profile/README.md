# AI Ecoverse

**The world's trailing AI Lab - Made with ❤️ in `Berlin` using military grade claude**

A comprehensive ecosystem of tools designed to enhance the AI-assisted development experience, improve transparency, and ensure proper attribution in AI-human collaborative coding.

## 🤖 Core AI Agent Tools

### [YOLO](https://github.com/ai-ecoverse/yolo)

![YOLO - AI CLI Wrapper with Worktree Isolation](https://raw.githubusercontent.com/ai-ecoverse/yolo/main/hero-banner.jpg)

AI CLI tool wrapper with worktree support. Launches AI coding assistants (Claude, Codex, Cursor, Gemini, etc.) with appropriate bypass flags and optional isolated git worktrees for safe experimentation. Supports multi-agent mode with parallel execution and automatic cleanup.

### [ai-aligned-git](https://github.com/ai-ecoverse/ai-aligned-git)

![AI-Aligned-Git](https://github.com/user-attachments/assets/38110bb1-c1d2-4e3d-ae58-2bebb18fe64c)

Git wrapper that enforces safe practices for AI coding agents. Prevents dangerous operations like `git add .`, ensures proper AI attribution, enforces commit hooks, and maintains human sign-off on all AI-generated commits.

### [ai-aligned-gh](https://github.com/ai-ecoverse/ai-aligned-gh)

![AI-Aligned-GH](https://github.com/user-attachments/assets/969463fc-4276-4ed1-8e20-6fee8aafeb3c)

Transparent GitHub CLI wrapper that automatically detects AI tool usage and ensures proper bot attribution. Uses device flow to exchange user tokens for bot tokens, so actions appear as "as-a-bot[bot] on behalf of @user" rather than appearing to come directly from the user.

### [as-a-bot](https://github.com/ai-ecoverse/as-a-bot)

![as-a-bot](https://raw.githubusercontent.com/ai-ecoverse/as-a-bot/main/hero-image.png)

GitHub App token broker running on Cloudflare Workers. Provides user-to-server GitHub tokens via device flow for ai-aligned-gh, ensuring actions show proper user attribution with app badges rather than appearing as bot-only actions.

### [military-grade-claude](https://github.com/ai-ecoverse/military-grade-claude)

![Military-Grade Claude](https://raw.githubusercontent.com/ai-ecoverse/military-grade-claude/main/hero-banner.jpg)

Tacticool upgrade patch for Claude Code that replaces soft spinner verbs with COMBAT-READY status messages. Transforms "Thinking..." into "Annihilating", "Exterminatus-Grade-Purification-Commencing", and absurdly over-the-top military-themed status updates. One-command installation for maximum operational readiness.

### [claude-trmnl-skill](https://github.com/ai-ecoverse/claude-trmnl-skill)

Claude Code skill for pushing status updates and action items to TRMNL e-ink displays via webhook API. Includes responsive templates for full screen (message + action items list), half screen (top/bottom split), and smaller layouts (message only), plus a comprehensive TRMNL Framework design system reference.

### [slicc](https://github.com/ai-ecoverse/slicc)

![slicc - Browser-Based Coding Agent](https://raw.githubusercontent.com/ai-ecoverse/slicc/main/hero-banner.png)

A browser-based coding agent that runs as a Chrome extension, CLI server, or Electron float. Runs Claude directly in the browser with full filesystem access, a WebAssembly shell, browser automation via CDP, and a complete suite of code editing tools. The self-licking ice cream cone - an AI coding agent that builds itself.

## 🛠️ Developer Productivity Tools

### [gh-workflow-peek](https://github.com/ai-ecoverse/gh-workflow-peek)

![GH Workflow Peek](https://github.com/user-attachments/assets/451a28c1-ccb5-4bae-bb16-b94b45f9cebf)

GitHub CLI extension that intelligently filters and highlights errors in GitHub Actions workflow logs by severity. Auto-detects failed PR checks, prioritizes errors (fatal → error → warn → fail), and shows context around matches. Perfect for developers and AI agents working with limited context windows.

### [gh-upskill](https://github.com/ai-ecoverse/gh-upskill)

![Upskill – Install Agent Skills](https://raw.githubusercontent.com/ai-ecoverse/gh-upskill/main/hero-banner.jpeg)

Quickly install Claude/Agent skills from other repositories. Works standalone or as a GitHub CLI extension. Copies skills, creates discovery scripts, and updates AGENTS.md with clear markers for idempotent updates.

### [gh-monday](https://github.com/ai-ecoverse/gh-monday)

![gh-monday - A robot cat that loves Mondays](https://raw.githubusercontent.com/ai-ecoverse/gh-monday/main/hero-banner.jpg)

Ranked GitHub triage as a `gh` extension. Shows what needs your attention now: PRs/issues waiting on you, work waiting on others, local repos behind, AI coding sessions to resume, categorized notifications, and cleanup candidates. "Garfield was wrong. Mondays are when everything gets sorted." Install with: `gh extension install ai-ecoverse/gh-monday`.

## 📊 Transparency & Analytics

### [vibe-coded-badge-action](https://github.com/ai-ecoverse/vibe-coded-badge-action)

![Vibe Coded Badge Action](https://github.com/user-attachments/assets/0350cfe6-7631-4613-aa3e-74e2bd53eda4)

GitHub Action that analyzes repository git history to determine what percentage of commits were made by AI tools. Generates dynamic badges showing AI contribution levels with smart logo selection based on the dominant AI tool (Claude, Cursor, Gemini, Copilot, etc.).

## 🔐 Security & Secrets

### [mcpecrets](https://github.com/ai-ecoverse/mcpecrets)

A lightweight MCP secrets manager that uses Cloudflare Workers for compute and GitHub for persistence. Stores secrets as GitHub Actions Secrets and retrieves them via triggered workflows with ephemeral key encryption. Exposes five MCP tools over OAuth 2.1 with dynamic client registration, working with any MCP-compatible client.

## 📚 Libraries

### [am-i-ai](https://github.com/ai-ecoverse/am-i-ai)

![am-i-ai](https://raw.githubusercontent.com/ai-ecoverse/am-i-ai/main/hero.png)

Lightweight shell library for detecting AI coding agents. Provides robust two-phase detection (environment variables + process tree) to identify when code is running under AI control. Powers the AI detection in ai-aligned-git and ai-aligned-gh.

## 🎯 Use Cases

- **Safe Experimentation**: Use YOLO with worktree mode to test AI-generated changes in isolation
- **Proper Attribution**: Ensure all AI contributions are clearly marked in git history and GitHub
- **Efficient Debugging**: Quickly find critical errors in CI/CD logs with gh-workflow-peek
- **Skill Sharing**: Share and install AI agent skills across projects with gh-upskill
- **Transparency**: Track and visualize AI contributions with vibe-coded-badge-action

## 🚀 Getting Started

Each tool can be installed independently. Visit the individual repository links above for detailed installation instructions and usage examples.

Most tools offer one-line installation:

```bash
# YOLO
curl -fsSL https://raw.githubusercontent.com/ai-ecoverse/yolo/main/install.sh | sh

# ai-aligned-git
curl -fsSL https://raw.githubusercontent.com/ai-ecoverse/ai-aligned-git/main/install.sh | sh

# ai-aligned-gh
curl -fsSL https://raw.githubusercontent.com/ai-ecoverse/ai-aligned-gh/main/install.sh | sh

# military-grade-claude
curl -fsSL https://raw.githubusercontent.com/ai-ecoverse/military-grade-claude/main/install.sh | sh

# gh-upskill
curl -fsSL https://raw.githubusercontent.com/ai-ecoverse/gh-upskill/main/install.sh | bash

# gh extensions
gh extension install ai-ecoverse/gh-workflow-peek
gh extension install ai-ecoverse/gh-upskill

# am-i-ai (detection library, used by ai-aligned-git/gh)
curl -fsSL https://raw.githubusercontent.com/ai-ecoverse/am-i-ai/main/install.sh | sh
```

## 🌟 Philosophy

These tools embrace **vibe coding** - a new AI-assisted software development paradigm where developers guide AI tools through natural language to build software. The ecosystem ensures:

1. **Transparency**: All AI contributions are clearly attributed
2. **Safety**: Dangerous operations are prevented or clearly flagged
3. **Accountability**: Human developers maintain oversight and sign-off
4. **Efficiency**: Tools reduce friction in AI-human collaboration
5. **Visibility**: Analytics show the real impact of AI on codebases

## 📄 License

All projects are open source under Apache 2.0 or MIT licenses. See individual repositories for details.

## 🤝 Contributing

Contributions are welcome across all projects! Please visit individual repositories to submit issues or pull requests.

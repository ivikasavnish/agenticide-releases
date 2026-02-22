# Agenticide v0.5.0 - Extension Marketplace Release

**Release Date:** 2026-02-22  
**Type:** Major Feature Release

## 🎉 What's New

### Extension Marketplace
The biggest feature in v0.5.0 is the **NPX-style extension marketplace** with 12 pre-built extensions:

```bash
agenticide search              # Browse all extensions
agenticide search security     # Search by keyword
agenticide info security       # Get extension details
agenticide install security    # Install extension
agenticide list                # List installed extensions
```

### Available Extensions

1. **security** - SAST scanning, secret detection, vulnerability checking
2. **code-analyzer** - Code complexity metrics, dead code detection
3. **project-runner** - Auto-detect project type and run commands
4. **web-search** - Multi-engine search with content fetching
5. **test-generator** - Automatically generate test cases
6. **git-ops** - Git operations and PR review automation
7. **ai-recipes** - Pre-built AI workflow templates
8. **deployment** - Multi-cloud deployment automation
9. **monitoring** - Health checks and alerting
10. **cost-controller** - Cost tracking and optimization
11. **db-analytics** - Database query and analysis
12. **ui-design** - Design system components

### Multi-Launch Modes

```bash
agenticide              # Default: CLI mode
agenticide window       # Full window mode
agenticide micro        # Compact overlay mode
agenticide server       # API server mode
agenticide web          # Web browser mode
```

### Beautiful Terminal UI
- Lipgloss styling for gorgeous output
- Tables, badges, panels, progress bars
- Color-coded status indicators
- Responsive layouts

## 📦 Installation

### Homebrew (macOS/Linux)
```bash
brew tap ivikasavnish/agenticide
brew install agenticide
```

### Direct Download
```bash
# Linux AMD64
curl -L https://github.com/ivikasavnish/agenticide-releases/releases/download/v0.5.0/agenticide-linux-amd64 -o agenticide
chmod +x agenticide
sudo mv agenticide /usr/local/bin/

# macOS ARM64
curl -L https://github.com/ivikasavnish/agenticide-releases/releases/download/v0.5.0/agenticide-darwin-arm64 -o agenticide
chmod +x agenticide
sudo mv agenticide /usr/local/bin/
```

## 🚀 Quick Start

```bash
# Browse extensions
agenticide search

# Install security extension
agenticide install security

# Start chat
agenticide chat

# Get help
agenticide --help
```

## 📊 Binaries

| Platform | Architecture | Size | Binary |
|----------|--------------|------|--------|
| macOS | ARM64 | 8.2 MB | agenticide-darwin-arm64 |
| macOS | AMD64 | 8.7 MB | agenticide-darwin-amd64 |
| Linux | AMD64 | 8.3 MB | agenticide-linux-amd64 |
| Linux | ARM64 | 8.0 MB | agenticide-linux-arm64 |
| Windows | AMD64 | 8.9 MB | agenticide-windows-amd64.exe |

## 🔧 Technical Details

- **Language:** Go 1.25+
- **UI Framework:** Lipgloss
- **CLI Framework:** Cobra
- **Storage:** SQLite (with CGO)
- **Binary Size:** 8-9 MB (standalone)
- **Dependencies:** None (static binary)

## 🆚 Comparison with v3.1.0

| Feature | v3.1.0 (Node.js) | v0.5.0 (Go) |
|---------|------------------|-------------|
| Extension Marketplace | ❌ | ✅ |
| Multi-launch Modes | ❌ | ✅ |
| Lipgloss UI | ❌ | ✅ |
| AI Chat | ✅ | ✅ |
| Code Analysis | ✅ | Via extension |
| Task Management | ✅ | ✅ |
| Signup/Licensing | ❌ | ✅ |

## 📝 Breaking Changes

None - this is a new implementation alongside v3.1.0.

## 🐛 Known Issues

- Requires CGO for SQLite support
- Building locally may have issues with mise-installed Go
- Use CI/CD or standard Go toolchain for builds

## 🔜 What's Next (v0.6.0)

- Extension SDK for custom extensions
- Extension marketplace API
- Remote extension registry
- Extension auto-updates
- Worker runner system
- Commercial licensing enforcement

## 📖 Documentation

- [Extension Contract](https://github.com/ivikasavnish/agenticide-go/blob/main/docs/EXTENSION_CONTRACT.md)
- [Homebrew Installation](https://github.com/ivikasavnish/agenticide-go/blob/main/HOMEBREW_INSTALL.md)
- [Marketplace Guide](https://github.com/ivikasavnish/agenticide-go/blob/main/MARKETPLACE.md)

## 🙏 Acknowledgments

Built with Go, Cobra, Lipgloss, and love for developer productivity.

---

**Full Changelog:** v3.1.0...v0.5.0

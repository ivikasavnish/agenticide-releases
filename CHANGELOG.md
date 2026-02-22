# Changelog

All notable changes to Agenticide will be documented in this file.

## [0.5.0] - 2026-02-22

### 🎉 Phase 4 Complete - Production Ready

**Full CLI Testing**
- Comprehensive testing of all commands
- Extension contract validation
- Error handling verification

**Documentation**
- Homebrew installation guide
- Extension contract documentation
- Phase completion summaries

### Changed
- Removed unused imports for cleaner codebase
- Finalized Phase 4 implementation
- Production-ready release

### Repository
- Source: https://github.com/ivikasavnish/agenticide-go
- Releases: https://github.com/ivikasavnish/agenticide-releases

---

## [0.4.0] - 2026-02-21

### 🎉 Major Features

**Extension Marketplace**
- npx-style extension discovery and installation
- 12 extensions in catalog (security, code-analyzer, web-search, etc.)
- Remote installation from GitHub/registry
- Tag-based search and category filtering
- Version management and progress indicators

**Default Chat**
- Just run `agenticide` (no args needed)
- Streamlined UX - chat is the primary interface

**Signup & Licensing**
- User registration with email, mobile, LinkedIn validation
- License key generation (AGNT-XXXX-XXXX format)
- Approval workflow with local storage

**Multiple Launch Modes**
- CLI mode (default)
- Window mode (full-screen TUI)
- Micro mode (floating overlay)
- Server mode (background daemon)
- Web mode (browser interface)

### Added
- `agenticide search [query]` - Search extension marketplace
- `agenticide install <ext>` - Install extension
- `agenticide list` - List installed extensions
- `agenticide info <ext>` - Extension details
- `agenticide uninstall <ext>` - Remove extension
- `agenticide signup` - User registration
- `agenticide activate <key>` - License activation
- `agenticide window/micro/web/server` - Launch modes
- Extension contract documentation (docs/EXTENSION_CONTRACT.md)
- Marketplace documentation (MARKETPLACE.md)

### Changed
- Default command is now chat (just run `agenticide`)
- Improved CLI structure with marketplace commands
- Enhanced README with marketplace features

### Repository
- Source: https://github.com/ivikasavnish/agenticide-go
- Releases: https://github.com/ivikasavnish/agenticide-releases

---

## [0.3.0] - 2026-02-14

### Added
- CLI commands: ext, task, chat, plan
- Extension management (list/enable/disable/info)
- Task management with dependency tracking
- Interactive chat with --ultraloop and --ultrathink
- Plan mode for task decomposition

### Changed
- Integrated all commands into main CLI
- Added beautiful terminal UI with Lipgloss

---

## [0.2.0] - 2026-02-12

### Added
- Terminal UI with 6 Lipgloss components
- Tables, progress bars, lists, panels, charts, badges
- Status icons (✓ ◐ ○ ⚠)
- Color themes and styles

---

## [0.1.0] - 2026-02-11

### Added
- Core extension system
- Context management
- SQLite storage with migrations
- Viper configuration
- Zap structured logging
- Event bus for inter-extension communication

---

## [v0.3.0] - 2026-02-21

### Added
- **CLI Commands**: Complete command suite (ext, task, chat, plan)
- **Task Management**: Dependency-aware task tracking with graph visualization
- **Interactive Chat**: REPL with ultraloop/ultrathink modes
- **Plan Mode**: Automatic task decomposition from requirements
- **Extension System**: Enable/disable extensions dynamically
- **Beautiful UI**: Lipgloss-styled tables, progress bars, lists, panels

### Core Infrastructure
- SQLite storage for persistence
- Viper configuration management
- Zap structured logging
- Context management with timeout/cancellation
- Event bus for inter-extension communication

## [v0.2.0] - 2026-02-21

### Added
- **Terminal UI Framework**: 6 reusable components
  - Table with alternating rows
  - Progress bar with percentage
  - List with status icons (✓ ◐ ○ ⚠)
  - Panel with borders
  - Bar chart with dynamic scaling
  - Sparkline for trends
- **Color Themes**: Purple, green, orange, red, blue, gray
- **Styles System**: Consistent Lipgloss styling

## [v0.1.0] - 2026-02-21

### Added
- **Extension Registry**: Thread-safe extension management
- **Event Bus**: Pub/sub messaging system
- **CLI Framework**: Cobra-based command structure
- **Core Interfaces**: Extension, Registry, EventBus, Context
- **Basic Commands**: version, help, chat
- **Super Keywords**: --ultraloop and --ultrathink flags

### Infrastructure
- Go module initialization
- Project structure setup
- Basic tests

---

## Upcoming

### [v0.4.0] - In Development
- Security Agent extension
- Code Analyzer extension  
- Project Runner extension
- Web Search extension
- Signup & approval system
- Window launcher modes

### [v0.5.0] - Planned
- LLM Agentic Recipes extension
- DB & Analytics extension
- Deployment Agent extension
- Cost Controller extension
- Proactive Monitoring extension
- UI Design extension

### [v1.0.0] - Roadmap
- Extension marketplace
- Commercial licensing
- API service mode
- Cloud sync
- Team collaboration features

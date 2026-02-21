# Changelog

All notable changes to Agenticide will be documented in this file.

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

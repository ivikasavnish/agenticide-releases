# Agenticide Releases

Pre-built binaries for [Agenticide](https://github.com/ivikasavnish/agenticide-go) - AI-powered development assistant.

## Download

### Latest Release

**macOS (Apple Silicon)**
```bash
curl -L https://github.com/ivikasavnish/agenticide-releases/releases/latest/download/agenticide-darwin-arm64 -o agenticide
chmod +x agenticide
sudo mv agenticide /usr/local/bin/
```

**macOS (Intel)**
```bash
curl -L https://github.com/ivikasavnish/agenticide-releases/releases/latest/download/agenticide-darwin-amd64 -o agenticide
chmod +x agenticide
sudo mv agenticide /usr/local/bin/
```

**Linux (x86_64)**
```bash
curl -L https://github.com/ivikasavnish/agenticide-releases/releases/latest/download/agenticide-linux-amd64 -o agenticide
chmod +x agenticide
sudo mv agenticide /usr/local/bin/
```

**Windows (x86_64)**
```powershell
# Download from releases page
# https://github.com/ivikasavnish/agenticide-releases/releases/latest
```

## Signup Required

Agenticide requires registration and approval for use.

### Registration

```bash
agenticide signup
```

You'll be prompted for:
- **Email**: Your work/personal email
- **Mobile**: Phone number with country code
- **LinkedIn**: Your LinkedIn profile URL
- **Use Case**: Brief description of intended use

### Approval Process

1. Submit registration form
2. Wait for approval (typically 24-48 hours)
3. Receive license key via email
4. Activate with: `agenticide activate <license-key>`

## Features

### Extension System
- **Security Agent** - SAST scanning, secret detection, vulnerability checks
- **Code Analyzer** - Complexity metrics, dead code detection
- **Project Runner** - Auto-detect and run any project type
- **Web Search** - Multi-engine search with content extraction
- **Task Management** - Dependency-aware task tracking
- **Interactive Chat** - AI-powered assistance with ultraloop/ultrathink modes

### Launch Modes

```bash
# CLI mode (default)
agenticide chat

# Full window mode (TUI)
agenticide --mode=window

# Micro window (floating overlay)
agenticide --mode=micro

# Server mode (background daemon)
agenticide server start
```

## System Requirements

- **macOS**: 10.15+ (Catalina or newer)
- **Linux**: Ubuntu 20.04+, Debian 11+, or equivalent
- **Windows**: Windows 10/11 (64-bit)
- **Memory**: 512MB minimum, 2GB recommended
- **Disk**: 50MB for binary + storage

## Verification

All binaries are signed and checksummed:

```bash
# Verify SHA256
curl -L https://github.com/ivikasavnish/agenticide-releases/releases/latest/download/SHA256SUMS
sha256sum -c SHA256SUMS

# Verify signature (GPG)
curl -L https://github.com/ivikasavnish/agenticide-releases/releases/latest/download/SHA256SUMS.sig
gpg --verify SHA256SUMS.sig SHA256SUMS
```

## License

Proprietary - Commercial use requires license.
See [LICENSE](../agenticide-go/LICENSE) for details.

## Support

- **Issues**: [GitHub Issues](https://github.com/ivikasavnish/agenticide-go/issues)
- **Docs**: [Documentation](https://github.com/ivikasavnish/agenticide-go/docs)
- **Email**: support@agenticide.dev

## Changelog

See [CHANGELOG.md](CHANGELOG.md) for release history.

## Build from Source

To build from source instead:
```bash
git clone https://github.com/ivikasavnish/agenticide-go
cd agenticide-go
go build -o agenticide ./cmd/agenticide
```

---

**Note**: This repository contains only pre-built binaries. 
Source code is at [ivikasavnish/agenticide-go](https://github.com/ivikasavnish/agenticide-go).

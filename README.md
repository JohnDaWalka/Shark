# Shark

A cross-platform repository with full Windows compatibility, designed for AIG intelligence integration.

## 🖥️ Platform Support

Shark is fully compatible with all major operating systems:

- ✅ **Windows** - Windows 10, Windows 11, Windows Server 2016+
- ✅ **Linux** - Ubuntu, Debian, RHEL, and other distributions
- ✅ **macOS** - macOS 10.15 and later

### Windows Users

For Windows-specific setup instructions, see [Windows Setup Guide](docs/WINDOWS_SETUP.md).

Quick start on Windows:
```powershell
# Clone the repository
git clone https://github.com/JohnDaWalka/Shark.git
cd Shark

# Run Windows setup script
.\scripts\setup-windows.ps1
```

Or using Command Prompt:
```cmd
scripts\setup-windows.bat
```

## 🚀 Quick Start

### Prerequisites

- Git installed on your system
- Your preferred development environment

### Installation

```bash
# Clone the repository
git clone https://github.com/JohnDaWalka/Shark.git

# Navigate to the project directory
cd Shark
```

## 🔧 Development

The repository includes cross-platform CI/CD workflows that test on:
- Windows (multiple versions)
- Linux (Ubuntu)
- macOS

See `.github/workflows/cross-platform.yml` for details.

## 📝 Code Quality

This repository uses [Sourcery AI](https://sourcery.ai/) for automated code review. Sourcery reviews all pull requests and provides suggestions for code improvements.

### Setup

To enable Sourcery on pull requests:
1. Add the `SOURCERY_TOKEN` secret to your repository settings
2. Get your token from [Sourcery Dashboard](https://app.sourcery.ai/)

You can also trigger a manual review by commenting `@sourcery-ai review` on any pull request.

## 📚 Documentation

- [Windows Setup Guide](docs/WINDOWS_SETUP.md) - Complete guide for Windows users
- [Contributing Guidelines](CONTRIBUTING.md) - How to contribute to this project

## 🤝 Contributing

Contributions are welcome! Please ensure your code works on all supported platforms:
1. Test on Windows, Linux, and macOS when possible
2. Follow the EditorConfig settings
3. Ensure all CI checks pass

## 📄 License

See [LICENSE](LICENSE) file for details.

## 🔗 Related Projects

This project integrates concepts from:
- Charcuterie repository principles
- Perplexity iOS app integrations
- AIG intelligence frameworks

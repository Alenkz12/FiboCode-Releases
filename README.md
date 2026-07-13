# FiboCode

FiboCode is a local-first AI code analysis desktop app that brings together a terminal, a code editor, and an AI chat to help you understand, analyze, and explore codebases right on your own machine. Your code and data never leave your computer.

> This is the **distribution repository** — it only hosts release binaries and update metadata. The source code lives elsewhere.

## Download & Install

Head to the [Releases](../../releases/latest) page and download the package that matches your platform.

| Platform | File | Notes |
| --- | --- | --- |
| macOS (Apple Silicon) | `FiboCode-<version>-arm64-mac.dmg` | For M1 / M2 / M3 / M4 chips |
| Windows | `FiboCode-Setup-<version>.exe` | 64-bit installer |
| Linux | `FiboCode-<version>-<arch>.AppImage` | Make it executable, then run |

### macOS

1. Open the `.dmg` and drag FiboCode into your Applications folder.
2. On first launch, if macOS says the developer cannot be verified, go to **System Settings → Privacy & Security** and click **Open Anyway**.

### Windows

Run the `.exe` installer and follow the setup wizard.

### Linux

```bash
chmod +x FiboCode-<version>-<arch>.AppImage
./FiboCode-<version>-<arch>.AppImage
```

## Auto Update

FiboCode checks this repository for new versions on startup. When an update is available, you can download and install it from within the app.

## License & Commercial Use

FiboCode is **free for personal use**. For enterprise or commercial use, please refer to the licensing terms in each release's notes.

## Feedback & Support

Run into a problem or have a feature request? Open an [Issue](../../issues) and let us know.

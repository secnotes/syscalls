# Linux Syscall Table

[English](README.md) | [中文](README_CN.md)

A comprehensive, interactive reference for Linux system calls across multiple architectures.

## Features

- **Multi-architecture Support**: x86, x86_64, arm, arm64
- **1,400+ Syscalls**: Complete syscall database with numbers, names, declarations, and descriptions
- **Search & Filter**: Quick lookup by name or syscall number, filter by architecture
- **Bilingual**: Chinese and English interface with automatic browser language detection
- **Dark Mode**: Automatic theme detection based on browser preferences
- **Responsive Design**: Works on desktop and mobile devices

## Usage

Open `index.html` in a web browser. No server required - it's a standalone HTML file with embedded data.

### Controls

- **Search**: Enter syscall name or number to filter results
- **Architecture Filter**: Select specific architecture (x86/x86_64/arm/arm64)
- **Language Toggle**: Switch between Chinese and English
- **Theme Toggle**: Switch between light and dark mode

## Data Source

System call data is sourced from [Chromium OS Docs - Linux System Call Table](https://chromium.googlesource.com/chromiumos/docs/+/master/constants/syscalls.md).

## Technical Details

- Pure static HTML, no external dependencies
- Embedded JSON data (~1,400 syscall entries)
- CSS with dark theme support
- JavaScript for filtering, rendering, and i18n
- ~412KB single-file application

## License

MIT

## Author

[Security Notes](https://github.com/secnotes)
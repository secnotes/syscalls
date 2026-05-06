# Linux Syscall Table

[English](README.md) | [中文](README_CN.md)

A comprehensive, interactive reference for Linux system calls across multiple architectures.

## Features

- **Multi-architecture Support**: x86, x86_64, arm, arm64, riscv32, riscv64, mips, mips64, powerpc, powerpc64, s390, s390x
- **4,400+ Syscalls**: Complete syscall database with numbers, names, declarations, and descriptions
- **Search & Filter**: Quick lookup by name or syscall number, filter by architecture
- **Bilingual**: Chinese and English interface with automatic browser language detection
- **Dark Mode**: Automatic theme detection based on browser preferences
- **Responsive Design**: Works on desktop and mobile devices

## Usage

Open `index.html` in a web browser. No server required - it's a standalone HTML file with embedded data.

### Controls

- **Search**: Enter syscall name or number to filter results
- **Architecture Filter**: Select specific architecture (x86/x86_64/arm/arm64/riscv32/riscv64/mips/mips64/powerpc/powerpc64/s390/s390x)
- **Language Toggle**: Switch between Chinese and English
- **Theme Toggle**: Switch between light and dark mode

## Data Source

- x86/x86_64/arm/arm64: [Chromium OS Docs - Linux System Call Table](https://chromium.googlesource.com/chromiumos/docs/+/master/constants/syscalls.md)
- riscv32/riscv64: Linux kernel `include/uapi/asm-generic/unistd.h`
- mips/mips64: Linux kernel `arch/mips/kernel/syscalls/syscall_o32.tbl` & `syscall_n64.tbl`
- powerpc/powerpc64: Linux kernel `arch/powerpc/kernel/syscalls/syscall.tbl`
- s390/s390x: Linux kernel `arch/s390/kernel/syscalls/syscall.tbl`

> If you need more detailed syscall source code mapping, check out [syscalls.mebeim.net](https://syscalls.mebeim.net).

## Technical Details

- Pure static HTML, no external dependencies
- Embedded JSON data (~4,400 syscall entries across 12 architectures)
- CSS with dark theme support
- JavaScript for filtering, rendering, and i18n
- ~1.2MB single-file application

## License

MIT

## Author

[Security Notes](https://github.com/secnotes)
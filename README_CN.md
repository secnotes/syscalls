# Linux 系统调用表

跨多架构的 Linux 系统调用交互式参考手册。

## 功能特性

- **多架构支持**：x86、x86_64、arm、arm64、riscv32、riscv64、mips、mips64、powerpc、powerpc64、s390、s390x
- **4400+ 系统调用**：完整的系统调用数据库，包含编号、名称、函数声明和描述
- **搜索与过滤**：按名称或编号快速查找，按架构筛选
- **双语支持**：中文和英文界面，自动检测浏览器语言
- **暗色主题**：根据浏览器偏好自动检测主题
- **响应式设计**：支持桌面和移动设备

## 使用方法

在浏览器中打开 `index.html`。无需服务器 - 这是一个嵌入数据的独立 HTML 文件。

### 控制选项

- **搜索**：输入系统调用名称或编号过滤结果
- **架构筛选**：选择特定架构（x86/x86_64/arm/arm64/riscv32/riscv64/mips/mips64/powerpc/powerpc64/s390/s390x）
- **语言切换**：切换中文和英文
- **主题切换**：切换亮色和暗色模式

## 数据来源

- x86/x86_64/arm/arm64：[Chromium OS Docs - Linux System Call Table](https://chromium.googlesource.com/chromiumos/docs/+/master/constants/syscalls.md)
- riscv32/riscv64：Linux 内核 `include/uapi/asm-generic/unistd.h`
- mips/mips64：Linux 内核 `arch/mips/kernel/syscalls/syscall_o32.tbl` & `syscall_n64.tbl`
- powerpc/powerpc64：Linux 内核 `arch/powerpc/kernel/syscalls/syscall.tbl`
- s390/s390x：Linux 内核 `arch/s390/kernel/syscalls/syscall.tbl`

> 如果你想要更详细的系统调用源码映射，请参考 [syscalls.mebeim.net](https://syscalls.mebeim.net)。

## 技术细节

- 纯静态 HTML，无外部依赖
- 嵌入式 JSON 数据（约 4400 条系统调用，覆盖 12 种架构）
- CSS 支持暗色主题
- JavaScript 实现过滤、渲染和国际化
- 单文件应用，约 1.2MB

## 许可证

MIT

## 作者

[Security Notes](https://github.com/secnotes)
<p align="center">
  <img src="icon/logo.png" alt="CytStudio Logo" width="128">
</p>

<h1 align="center">CytStudio</h1>

<p align="center">
  <strong>An Embedded Development IDE</strong><br>
  <sub>AI Agent · Debugger · Code Analysis · Built for MCU/Embedded Engineers</sub>
</p>

<p align="center">
  <a href="#-key-features">Features</a> •
  <a href="#-quick-start">Quick Start</a> •
  <a href="#-build-from-source">Build</a> •
  <a href="#-architecture">Architecture</a> •
  <a href="#-license">License</a>
</p>

---

## 📖 Introduction

**CytStudio** is an embedded development IDE built by a solo developer, exploring what an alternative tool outside the mainstream could look like. It tries to bring together an AI coding agent, a hardware-aware debugger, static code analysis, and everyday project tooling in one place — not to replace the tools you already trust, but to offer another option worth trying.

If you work with ARM Cortex-M, FreeRTOS, or bare-metal projects, CytStudio supports importing from CubeMX, IAR, and Keil, J-Link debugging with FreeRTOS awareness, and an AI agent that can read, write, build, and debug code alongside you. It's a personal project, a constant work in progress, and always open to feedback.

---

## ✨ Key Features

### 🤖 AI Agent
- **Multi-Provider**: Anthropic Claude, Kimi/Moonshot, DeepSeek, and extensible provider architecture
- **Rich Tool System**: 50+ tool categories — file ops, search, git, build, Python/Bash execution, PDF, Excel, MCP resources
- **Agent Team Orchestration**: Multi-agent collaboration with pipelines, sub-agents, and task orchestration
- **MCP Protocol**: Full Model Context Protocol support (stdio + HTTP transports)
- **Skill System**: User-defined and project-level skills with hot reload
- **RAG Memory**: Hybrid retrieval (BM25 + semantic + reranking), episodic memory, implicit context
- **Streaming Output**: Real-time token streaming with collapsible thinking blocks
- **Audit Logging**: Full compliance trail with timeline viewer and HTML report export
- **Permission System**: Trust-gradient permission model with user confirmation dialogs
- **Multi-Session**: Fully isolated parallel chat sessions with independent StreamControllers

### 🔍 Code Analysis (In Refinement)
- **Call Graph**: Interactive bezier-curve call graph with expand/collapse
- **Control Flow Graph**: Per-function CFG extraction and visualization
- **Code Metrics**: Cyclomatic complexity, Halstead metrics, nesting depth, LOC
- **Duplicate Detection**: Cross-file duplicate code detection
- **Inheritance / Include Analysis**: Class hierarchy and include graph visualization
- **Export**: Image (PNG/SVG), HTML report, CSV data export

### 🐛 Hardware Debugger
- **J-Link Interface**: Full J-Link integration with hardware mutex
- **FreeRTOS Dashboard**: Task list, stack usage, runtime stats
- **Breakpoints & Watchpoints**: Conditional breakpoints, data watchpoints
- **Variable Inspection**: Tree-structured live variable view
- **Disassembly**: Mixed source/assembly view
- **Memory View**: Hex dump with configurable columns
- **Register View**: CPU and peripheral register inspection
- **Call Stack**: Frame-accurate stack trace with DWARF resolution
- **High-Speed Sampling**: Microsecond-level data sampling & waveform

### 📝 Code Editor
- **Clang-Based Completion**: Semantic code completion via libclang
- **Syntax Highlighting**: Full C/C++ highlighting with semantic token coloring
- **Minimap**: Code overview minimap with scroll synchronization
- **Symbol Outline**: File structure outline for quick navigation
- **Multi-File Search**: Project-wide regex search with result panel
- **Markdown & PDF**: Built-in markdown preview and PDF viewer

### 🔧 Build System
- **Build Diagnostics**: Parsed compiler errors/warnings with source navigation
- **Async Build**: Non-blocking build execution with streaming output
- **Project Config**: Toolchain and build configuration management

### 📦 Project Management
- **Project Migration**: Import from **STM32CubeMX**, **IAR EWARM**, **Keil MDK**
- **Git Integration**: Built-in git operations, diff viewer, log graph, terminal
- **Recent Projects**: Quick-access recent project list
- **Theme System**: Light/dark theme with accent color customization

### 📊 Data Visualization
- **Real-Time Waveform**: Oscilloscope-style data plotting with measurement tools
- **Legend & Cursor**: Highlightable legend, multi-cursor measurement
- **Data Export**: CSV export for captured waveform data

### 🔐 License & Activation
- **Online Activation**: Secure hardware-bound license activation
- **Runtime Guard**: Continuous license validation during operation

---

## 🚀 Quick Start

### Download

Get the latest installer from [GitHub Releases](https://github.com/cytstudiooo/cytstudio/releases).

- **CytStudio_Setup_Vx.x.x.exe** — Windows installer with modern wizard UI

### System Requirements

| Requirement | Minimum |
|-------------|---------|
| OS | Windows 10 / 11 (x64) |
| RAM | 4 GB |
| Disk | 3 GB free |

### Installation

1. Download `CytStudio_Setup_V2.3.5.exe`
2. Run the installer and follow the wizard
3. Launch from desktop shortcut or Start Menu

---

## 🔨 Build from Source

### Prerequisites

- **Qt 6.10+** (MinGW 64-bit on Windows)
- **LLVM/Clang 18+** (for code completion and analysis)
- **Vulkan SDK 1.4+** (for llama.cpp GPU inference)
- **J-Link** (for debugger features)

---

## 🔌 Supported File Associations

| Extension | Description |
|-----------|-------------|
| `.rproj` | CytStudio Run Configuration File |
| `.cproj` | CytStudio Project File |

---

## 📄 License

© 2024–2026 CytStudio. All rights reserved.

This project is proprietary software. See the license terms provided with your installation.

---

## 📧 Contact

- **Email**: [cyte_studio@foxmail.com](mailto:cyte_studio@foxmail.com)
- **Author**: [mjkun](https://github.com/mjkun)

---

<p align="center">
  <sub>Built with Qt 6 · C++17 · QML · LLVM/Clang · J-Link · llama.cpp</sub>
</p>

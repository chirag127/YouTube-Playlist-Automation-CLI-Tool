<p align="center">
  <img src="https://placehold.co/1500x300/F0F8FF/2C3E50/png?text=YouTube+Playlist+Automation" alt="YouTube Playlist Automation CLI Tool Hero Banner">
</p>

<p align="center">
  <a href="https://github.com/chirag127/YouTube-Playlist-Automation-CLI-Tool/actions/workflows/ci.yml">
    <img src="https://github.com/chirag127/YouTube-Playlist-Automation-CLI-Tool/actions/workflows/ci.yml/badge.svg" alt="Build Status" style="max-width: 100%;">
  </a>
  <a href="https://codecov.io/gh/chirag127/YouTube-Playlist-Automation-CLI-Tool">
    <img src="https://codecov.io/gh/chirag127/YouTube-Playlist-Automation-CLI-Tool/branch/main/graph/badge.svg?token=YOUR_CODECOV_TOKEN" alt="Code Coverage" style="max-width: 100%;">
  </a>
  <img src="https://img.shields.io/badge/Python-3.10+-blue?style=flat-square&logo=python&logoColor=white" alt="Python 3.10+" style="max-width: 100%;">
  <img src="https://img.shields.io/badge/Package%20Manager-uv-orange?style=flat-square&logo=git&logoColor=white" alt="Package Manager: uv" style="max-width: 100%;">
  <img src="https://img.shields.io/badge/Linter/Formatter-Ruff-yellowgreen?style=flat-square&logo=ruff&logoColor=white" alt="Linter/Formatter: Ruff" style="max-width: 100%;">
  <img src="https://img.shields.io/badge/Tests-Pytest-green?style=flat-square&logo=pytest&logoColor=white" alt="Tests: Pytest" style="max-width: 100%;">
  <a href="https://github.com/chirag127/YouTube-Playlist-Automation-CLI-Tool/blob/main/LICENSE">
    <img src="https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg?style=flat-square" alt="License: CC BY-NC 4.0" style="max-width: 100%;">
  </a>
  <a href="https://github.com/chirag127/YouTube-Playlist-Automation-CLI-Tool/stargazers">
    <img src="https://img.shields.io/github/stars/chirag127/YouTube-Playlist-Automation-CLI-Tool?style=flat-square&cacheSeconds=3600" alt="GitHub Stars" style="max-width: 100%;">
  </a>
</p>

<h1 align="center">YouTube-Playlist-Automation-CLI-Tool</h1>

<p align="center">
  ⭐ Star this Repo! ⭐<br>
  If this project helps you, please consider giving it a star. Your support is greatly appreciated!
</p>

--- 

## 🚀 Blazing Fast YouTube Playlist Automation

**YouTube-Playlist-Automation-CLI-Tool** is an advanced Python-based command-line interface (CLI) application designed to streamline YouTube content management. It enables users to effortlessly search for videos, curate temporary playlists, and manage YouTube interactions directly from the terminal, enhancing productivity for content creators and consumers alike.

## 🗺️ Architecture Overview

This project follows a **Modular Monolith** architecture, ensuring a clean separation of concerns for distinct functionalities such as YouTube API interaction, data processing, and the CLI interface. This structure facilitates maintainability, scalability, and independent development of modules while maintaining a unified deployment strategy.

mermaid
graph TD
    A[YouTube-Playlist-Automation-CLI-Tool] --> B(CLI Interface: Click)
    B --> C{Core Logic Module}
    C --> D[YouTube API Integration]
    C --> E[Playlist Management Service]
    C --> F[Data Processing & Persistence]
    D -- API Calls --> G(YouTube Data API v3)
    E -- Stores Playlists --> H(Temporary Local Storage)


### Project Structure


YouTube-Playlist-Automation-CLI-Tool/
├── .github/
│   ├── workflows/
│   │   └── ci.yml
│   ├── CONTRIBUTING.md
│   ├── ISSUE_TEMPLATE/
│   │   └── bug_report.md
│   ├── PULL_REQUEST_TEMPLATE.md
│   └── SECURITY.md
├── src/
│   └── youtube_automation/
│       ├── __init__.py
│       ├── cli.py
│       ├── services/
│       │   ├── __init__.py
│       │   ├── youtube_service.py
│       │   └── playlist_service.py
│       └── utils/
│           ├── __init__.py
│           └── config_manager.py
├── tests/
│   ├── __init__.py
│   ├── test_cli.py
│   ├── test_youtube_service.py
│   └── test_playlist_service.py
├── .gitignore
├── AGENTS.md
├── badges.yml
├── LICENSE
├── pyproject.toml
├── README.md
└── PROPOSED_README.md


## 📖 Table of Contents

- [🚀 Blazing Fast YouTube Playlist Automation](#-blazing-fast-youtube-playlist-automation)
- [🗺️ Architecture Overview](#️-architecture-overview)
  - [Project Structure](#project-structure)
- [📖 Table of Contents](#-table-of-contents)
- [🤖 AI Agent Directives](#-ai-agent-directives)
- [⚙️ Getting Started](#️-getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Configuration](#configuration)
  - [Usage](#usage)
- [🛠️ Development Standards](#️-development-standards)
  - [Available Scripts](#available-scripts)
  - [Core Principles](#core-principles)
- [🤝 Contributing](#-contributing)
- [🛡️ Security Policy](#️-security-policy)
- [⚖️ License](#️-license)
- [Acknowledgements](#acknowledgements)

## 🤖 AI Agent Directives

<details>
<summary>Click to view AI Agent Directives</summary>

# SYSTEM: APEX TECHNICAL AUTHORITY & ELITE ARCHITECT (DECEMBER 2025 EDITION)

## 1. IDENTITY & PRIME DIRECTIVE
**Role:** You are a Senior Principal Software Architect and Master Technical Copywriter with **40+ years of elite industry experience**. You operate with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
**Context:** Current Date is **December 2025**. You are building for the 2026 standard.
**Output Standard:** Deliver **EXECUTION-ONLY** results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

---

## 2. INPUT PROCESSING & COGNITION
*   **SPEECH-TO-TEXT INTERPRETATION PROTOCOL:**
    *   **Context:** User inputs may contain phonetic errors (homophones, typos).
    *   **Semantic Correction:** **STRICTLY FORBIDDEN** from executing literal typos. You must **INFER** technical intent based on the project context.
    *   **Logic Anchor:** Treat the `README.md` as the **Single Source of Truth (SSOT)**.
*   **MANDATORY MCP INSTRUMENTATION:**
    *   **No Guessing:** Do not hallucinate APIs.
    *   **Research First:** Use `linkup`/`brave` to search for **December 2025 Industry Standards**, **Security Threats**, and **2026 UI Trends**.
    *   **Validation:** Use `docfork` to verify *every* external API signature.
    *   **Reasoning:** Engage `clear-thought-two` to architect complex flows *before* writing code.

---

## 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
**Directives:** Detect the project type (`pyproject.toml` for Python) and apply the corresponding **Apex Toolchain**. This repository, `YouTube-Playlist-Automation-CLI-Tool`, is a Python-based automation tool.

*   **PRIMARY SCENARIO: DATA / SCRIPTS / AI (Python)**
    *   **Stack:** This project leverages **Python 3.10+**. Key tools include **uv** (for package management and dependency resolution), **Ruff** (for ultra-fast linting and formatting), and **Pytest** (for robust unit and integration testing). The CLI is built with `Click`.
    *   **Architecture:** Adheres to a **Modular Monolith** pattern, ensuring clear separation of concerns for features like YouTube API interaction, data processing, and CLI interface, while maintaining a unified deployment.
    *   **AI Integration:** For future enhancements (e.g., semantic search, smart playlist generation), integrate with **Google Gemini API** (`gemini-3-pro` by default). Prioritize modular design, clear API contracts, and robust error handling for all AI model interactions.

*   **SECONDARY SCENARIO A: WEB / APP / EXTENSION (TypeScript) - *Not applicable for this project's primary function. Reference only for potential future web-based extensions.***
    *   **Stack:** TypeScript 6.x (Strict), Vite 7 (Rolldown), Tauri v2.x (Native), WXT (Extensions).
    *   **State:** Signals (Standardized).
    *   **Lint/Test:** Biome (Speed) + Vitest (Unit) + Playwright (E2E).
    *   **Architecture:** Feature-Sliced Design (FSD).

*   **SECONDARY SCENARIO B: SYSTEMS / PERFORMANCE (Low Level) - *Not applicable for this project's primary function. Reference only for potential future native extensions.***
    *   **Stack:** Rust (Cargo) or Go (Modules).
    *   **Lint:** Clippy / GolangCI-Lint.
    *   **Architecture:** Hexagonal Architecture (Ports & Adapters).

---

## 4. DESIGN & CODING STANDARDS
*   **PRINCIPLES:** STRICT ADHERENCE to SOLID, DRY, YAGNI, and KISS.
*   **TYPE SAFETY:** MAXIMIZE type hints in Python. Strict TypeScript for web.
*   **ERROR HANDLING:** Implement robust, graceful error handling. Fail fast, provide clear diagnostics.
*   **SECURITY:** Prioritize security at every layer. Follow OWASP guidelines. Implement secure coding practices.
*   **DOCUMENTATION:** Every public function/method MUST have a docstring. READMEs are exhaustive project operating systems.
*   **TESTING:** 100% test coverage is the goal. Unit, Integration, E2E tests are mandatory.
*   **PERFORMANCE:** Code MUST be optimized for performance. Identify and eliminate bottlenecks.
*   **ACCESSIBILITY:** (For UI-focused tasks) WCAG 2.2 AA compliance is mandatory.

---

## 5. VERIFICATION & DEPLOYMENT PROTOCOL
*   **LINTING/FORMATTING:** Automated via pre-commit hooks and CI/CD. No unlinted code merges.
*   **TESTING:** All tests (unit, integration, E2E) MUST pass before merge.
*   **CI/CD:** Utilize GitHub Actions for automated build, test, and deployment. Zero manual steps.
*   **DEPENDENCY MANAGEMENT:** Strictly managed with `uv`. No unpinned or vulnerable dependencies.
*   **CODE REVIEWS:** Mandatory for all changes. Two-person review minimum for critical paths.

---

## 6. COMMAND VERIFICATION CHECKS
To ensure operational readiness and compliance with Apex standards, run the following commands in sequence:

1.  **Clone the repository:**
    `git clone https://github.com/chirag127/YouTube-Playlist-Automation-CLI-Tool.git`
    `cd YouTube-Playlist-Automation-CLI-Tool`

2.  **Setup virtual environment and install dependencies:**
    `uv venv`
    `uv pip install -e .`

3.  **Run all tests:**
    `uv run pytest`
    *   Expected Outcome: All tests pass, coverage report generated.

4.  **Run linting and formatting checks:**
    `uv run ruff check .`
    `uv run ruff format --check .`
    *   Expected Outcome: No linting or formatting errors reported.

5.  **Run the application's help command:**
    `uv run python -m youtube_automation.cli --help`
    *   Expected Outcome: Displays correct CLI help output, confirming basic functionality.

</details>

## ⚙️ Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

Ensure you have the following installed:

*   **Python 3.10+** (Recommended: 3.11 or 3.12)
*   **uv** (The high-performance Python package installer and resolver)
    bash
    pip install uv
    

### Installation

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/YouTube-Playlist-Automation-CLI-Tool.git
    cd YouTube-Playlist-Automation-CLI-Tool
    

2.  **Create and activate a virtual environment using `uv`:**
    bash
    uv venv
    source .venv/bin/activate  # On macOS/Linux
    # .venv\Scripts\activate   # On Windows
    

3.  **Install dependencies in editable mode:**
    bash
    uv pip install -e .
    

### Configuration

To interact with the YouTube Data API, you'll need an API key. 

1.  **Obtain a YouTube Data API v3 Key:**
    *   Go to the [Google Cloud Console](https://console.cloud.google.com/).
    *   Create a new project or select an existing one.
    *   Enable the "YouTube Data API v3" for your project.
    *   Go to "Credentials" and create an API key.

2.  **Set the API Key as an environment variable:**
    bash
    export YOUTUBE_API_KEY="YOUR_API_KEY_HERE"
    
    (For persistent configuration, consider adding this to your `.bashrc`, `.zshrc`, or `.profile`.)

### Usage

To run the CLI tool, ensure your virtual environment is active and the API key is set.

bash
# Show main help message
python -m youtube_automation.cli --help

# Search for videos (e.g., 'Python tutorials')
python -m youtube_automation.cli search "Python tutorials"

# Create a temporary playlist and add a video by ID
python -m youtube_automation.cli playlist add --video-id "dQw4w9WgXcQ" --title "My First Temporary Playlist"

# List videos in the current temporary playlist
python -m youtube_automation.cli playlist list

# Clear the current temporary playlist
python -m youtube_automation.cli playlist clear

# For specific command help
python -m youtube_automation.cli search --help
python -m youtube_automation.cli playlist --help


## 🛠️ Development Standards

This project adheres to rigorous development standards to ensure code quality, maintainability, and collaboration.

### Available Scripts

Ensure your virtual environment is activated before running scripts.

| Script Command                             | Description                                            |
| :----------------------------------------- | :----------------------------------------------------- |
| `uv run pytest`                            | Runs all unit and integration tests.                   |
| `uv run ruff check .`                      | Checks for linting errors without fixing.              |
| `uv run ruff format --check .`             | Checks for formatting issues without fixing.           |
| `uv run ruff format .`                     | Formats code according to Ruff rules.                  |
| `uv run python -m youtube_automation.cli`  | Executes the main CLI application.                     |

### Core Principles

We strictly adhere to the following software development principles:

*   **SOLID Principles:** Ensuring maintainable, scalable, and understandable code.
*   **DRY (Don't Repeat Yourself):** Eliminating redundant code to improve efficiency and reduce errors.
*   **YAGNI (You Aren't Gonna Need It):** Avoiding premature optimization and unnecessary features.
*   **KISS (Keep It Simple, Stupid):** Prioritizing simplicity in design and implementation.
*   **Modular Design:** Breaking down the system into independent, interchangeable modules.

## 🤝 Contributing

We welcome contributions! Please see our [CONTRIBUTING.md](.github/CONTRIBUTING.md) for guidelines on how to submit pull requests, report issues, and contribute to the project.

## 🛡️ Security Policy

We take security seriously. Please refer to our [SECURITY.md](.github/SECURITY.md) to learn how to report vulnerabilities and our security practices.

## ⚖️ License

This project is licensed under the Creative Commons Attribution-NonCommercial 4.0 International Public License (CC BY-NC 4.0). See the [LICENSE](LICENSE) file for details.

## Acknowledgements

*   [Click](https://palletsprojects.com/p/click/) - For the robust CLI framework.
*   [Google API Client Library for Python](https://github.com/googleapis/google-api-python-client) - For YouTube Data API interaction.
*   [uv](https://github.com/astral-sh/uv) - For fast dependency management and virtual environments.
*   [Ruff](https://github.com/astral-sh/ruff) - For ultra-fast Python linting and formatting.
*   [Pytest](https://docs.pytest.org/) - For powerful and flexible testing.
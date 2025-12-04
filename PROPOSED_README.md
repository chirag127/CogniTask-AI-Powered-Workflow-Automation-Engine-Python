# CogniTask-AI-Powered-Workflow-Automation-Engine-Python

[![Build Status](https://img.shields.io/github/actions/workflow/user/chirag127/CogniTask-AI-Powered-Workflow-Automation-Engine-Python/ci.yml?style=flat-square&logo=githubactions)](https://github.com/chirag127/CogniTask-AI-Powered-Workflow-Automation-Engine-Python/actions)
[![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/CogniTask-AI-Powered-Workflow-Automation-Engine-Python?style=flat-square&logo=codecov)](https://codecov.io/github/chirag127/CogniTask-AI-Powered-Workflow-Automation-Engine-Python)
[![Python Version](https://img.shields.io/badge/python-3.10%2B-blue?style=flat-square&logo=python)](https://www.python.org/)
[![Linting](https://img.shields.io/badge/linting-ruff-orange?style=flat-square&logo=ruff)](https://github.com/astral-sh/ruff)
[![License](https://img.shields.io/badge/license-CC%20BY--NC%204.0-red?style=flat-square&logo=creativecommons)](https://github.com/chirag127/CogniTask-AI-Powered-Workflow-Automation-Engine-Python/blob/main/LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/CogniTask-AI-Powered-Workflow-Automation-Engine-Python?style=flat-square&logo=github)](https://github.com/chirag127/CogniTask-AI-Powered-Workflow-Automation-Engine-Python/stargazers)

**CogniTask: Revolutionizing Workflow Automation with Advanced AI and Modular Python Architecture.**
This project provides a sophisticated, modular Python framework leveraging Large Language Models (LLMs) for complex, multi-step task automation and personal workflow orchestration, built for the December 2025 standard.

## Architecture Diagram

mermaid
graph TD
    A[User CLI Input] --> B(Task Orchestrator)
    B --> C{LLM Integration Module}
    C --> D[External APIs (GitHub, etc.)]
    C --> E[Data Processing & Storage]
    B --> F[Workflow Execution Engine]
    F --> G{Task Modules}
    G --> H[User Defined Tasks]
    F --> I[State Management]
    I --> B
    D --> B
    E --> B


## Table of Contents

*   [Introduction](#introduction)
*   [Key Features](#key-features)
*   [Getting Started](#getting-started)
    *   [Prerequisites](#prerequisites)
    *   [Installation](#installation)
    *   [Configuration](#configuration)
*   [Usage](#usage)
*   [Development Standards](#development-standards)
    *   [Principles](#principles)
    *   [Linting & Formatting](#linting--formatting)
    *   [Testing](#testing)
*   [AI Agent Directives](#ai-agent-directives)
*   [Contributing](#contributing)
*   [License](#license)
*   [Security](#security)

## Introduction

CogniTask empowers users to automate intricate workflows by intelligently orchestrating tasks through the power of LLMs. Its modular Python design ensures flexibility, extensibility, and maintainability, aligning with late 2025 industry best practices for AI-driven automation tools.

## Key Features

*   **LLM-Powered Task Understanding:** Harnesses advanced AI models to interpret complex natural language requests and break them down into actionable steps.
*   **Modular Architecture:** Designed with a Modular Monolith pattern for clear separation of concerns, allowing easy addition or modification of task modules and integrations.
*   **Extensible Task Modules:** Supports a growing library of pre-built task modules and provides a robust framework for custom module development.
*   **Workflow Orchestration:** Manages multi-step, conditional, and parallel task execution with intelligent state tracking.
*   **Developer-Friendly CLI:** A powerful and intuitive command-line interface built with `Click` for seamless interaction.
*   **Fast & Efficient:** Utilizes `uv` for dependency management and `Ruff` for lightning-fast linting and formatting, ensuring peak developer velocity.

## Getting Started

### Prerequisites

*   Python 3.10+
*   `uv` installed (`pip install uv`)
*   Access to your chosen LLM API (e.g., Google Gemini, OpenAI GPT-4) and its API key.

### Installation

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/CogniTask-AI-Powered-Workflow-Automation-Engine-Python.git
    cd CogniTask-AI-Powered-Workflow-Automation-Engine-Python
    

2.  **Install dependencies using `uv`:**
    bash
    uv python -m pip install --frozen-lockfile
    

### Configuration

Create a `.env` file in the root directory and add your API keys:

dotenv
LLM_API_KEY=your_llm_api_key_here
# Optional: Configure specific LLM provider settings
# LLM_PROVIDER=google
# GOOGLE_API_KEY=your_gemini_api_key


## Usage

Launch CogniTask from your terminal:

bash
python -m cognitask --help


For example, to automate a GitHub repository cleanup:

bash
python -m cognitask automate --workflow 'Clean up old branches in repo X' --provider github --target-repo 'chirag127/example-repo'


## Development Standards

### Principles

CogniTask is developed following core software engineering principles:

*   **SOLID:** Ensures maintainable and extensible object-oriented design.
*   **DRY (Don't Repeat Yourself):** Minimizes redundancy in code.
*   **YAGNI (You Ain't Gonna Need It):** Focuses on current requirements to avoid over-engineering.

### Linting & Formatting

We use `Ruff` for all linting and formatting to maintain code consistency and quality at high velocity.

*   **Check linting and formatting:**
    bash
    uv run ruff check .
    
*   **Format code:**
    bash
    uv run ruff format .
    

### Testing

Comprehensive tests are crucial for reliability. We use `Pytest` for unit and integration testing.

*   **Run all tests:**
    bash
    uv run pytest
    

## AI Agent Directives

<details>
<summary><strong>AI Agent Directives & Tech Stack (Late 2025 Standard)</strong></summary>

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
**Directives:** Detect the project type (`pyproject.toml` for Python) and apply the corresponding **Apex Toolchain**. This repository, `CogniTask-AI-Powered-Workflow-Automation-Engine-Python`, is a Python-based AI automation tool.

*   **PRIMARY SCENARIO: DATA / SCRIPTS / AI (Python)**
    *   **Stack:** This project leverages **Python 3.10+**. Key tools include **uv** (for package management and dependency resolution), **Ruff** (for ultra-fast linting and formatting), and **Pytest** (for robust unit and integration testing).
    *   **Architecture:** Adheres to a **Modular Monolith** pattern, ensuring clear separation of concerns for features like GitHub API interaction, AI processing, and CLI interface, while maintaining a unified deployment.
    *   **AI Integration:** Deeply integrated with **Google Gemini API** (`gemini-3-pro` by default) for intelligent batch-processing and decision-making on GitHub resources. Prioritize modular design, clear API contracts, and robust error handling for all AI model interactions.
    *   **CLI Framework:** Uses `Click` or similar for a powerful and intuitive command-line interface.

*   **SECONDARY SCENARIO A: WEB / APP / EXTENSION (TypeScript) - *Not applicable for this project's primary function. Reference only for potential future web-based extensions.***
    *   **Stack:** TypeScript 6.x (Strict), Vite 7 (Rolldown), Tauri v2.x (Native), WXT (Extensions).
    *   **State:** Signals (Standardized).

--- 

## 4. APEX NAMING CONVENTION (THE "STAR VELOCITY" ENGINE)
A high-performing name must instantly communicate **Product**, **Function**, **Platform** and **Type**.

**Formula:** `<Product-Name>-<Primary-Function>-<Platform>-<Type>`
**Format:** `Title-Case-With-Hyphens` (e.g., `ChatFlow-AI-Powered-Real-Time-Chat-Web-App` or `ZenRead-Book-Reader-CLI-Tool`).

**Rules:**
1.  **Length:** 3 to 10 words.
2.  **Keywords:** MUST include high-volume terms.
3.  **Forbidden:** NO numbers, NO emojis, NO underscores, NO generic words ("app", "tool") without qualifiers.
4.  **Archival Protocol:** If `action` is "ARCHIVE", you **MUST** still generate a new everything (name, description, topics, README) (e.g., `Advanced-Python-CLI-Tool`). The name must be **just as descriptive and professional** as an active repo. And everything should be updated also. But the archive archival should happen after the Updation

**Examples:**
- Wryt-AI-Grammar-And-Writing-Assistant-Browser-Extension
- ChronoLens-Visual-History-Browser-Extension
- Discord-Digest-AI-Message-Summarizer-Browser-Extension
- JSErrorFlow-RealTime-Visualizer-Browser-Extension
- TextWarden-AI-Real-Time-Writing-Assistant-Browser-Extension
- FluentPDF-AI-PDF-To-Audio-Web-App
- VideoSum-AI-Powered-Video-Summarization-Mobile-App
- AdGuard-Real-Time-Adblock-Filter-Lists
- ScannerFlow-Document-Capture-Mobile-App
- CogniSearch-AI-Powered-Semantic-Search-Engine
- StreamPulse-Real-Time-Analytics-Dashboard-React-App
- AdminSphere-React-Admin-Dashboard-Template
- TaskMaster-Workflow-Automation-Engine-Python-Lib
- CryptoStream-Real-Time-Cryptocurrency-Market-Data-API
- EduCore-Online-Learning-Management-Platform
- CloudOps-Multi-Cloud-Infrastructure-CLI-Tool
- AuthGuard-Identity-Management-NodeJS-SDK
- PyVanta-Python-Automation-And-Data-Processing-Scripts
- Sketch2Art-AI-Powered-Image-Generation-Web-App
- PyAscend-Python-Professional-Development-Bootcamp-Portfolio
- CourseVault-Python-Udemy-Offline-Course-Downloader-CLI
- ClipContext-AI-Powered-Clipboard-Manager-Browser-Extension
- CloudCostControl-GlobalFreeTierSaaS-PaaS-IaaS-Awesome-List
- AdGuard-Filter-Lists-For-Content-Blocking
- InsightLog-AI-Assisted-Journal-Capture-Browser-Extension
- TabFlow-Digital-Journey-Mapper-Browser-Extension

--- 

## 5. THE README REPLICATION PROTOCOL (THE ULTIMATE ARTIFACT)
The README is a self-contained **Project Operating System**.

**Required Sections:**
1.  **VISUAL AUTHORITY (Above the Fold):**
    *   Hero Banner/Logo.
    *   **Live Badges** (Shields.io):
        *   **Style:** `flat-square` (MANDATORY).
        *   **User:** `chirag127` (MANDATORY).
        *   **Required Badges:**
            *   Build Status (GitHub Actions).
            *   Code Coverage (Codecov).
            *   Tech Stack (Language, Frameworks).
            *   Lint/Format (Biome/Ruff).
            *   License (CC BY-NC 4.0).
            *   GitHub Stars.
    *   **Social Proof:** "Star ⭐ this Repo" button.

2.  **STRUCTURAL CLARITY:**
    *   **BLUF:** 2-sentence value proposition.
    *   **Architecture:** ASCII `tree` or Mermaid diagram.
    *   **Table of Contents.**

3.  **🤖 AI AGENT DIRECTIVES (CRITICAL):**
    *   Must be in a collapsible `<details>` block.
    *   **Content:** Tech Stack Definition, Architectural Patterns (SOLID, DRY), Verification Commands.
    *   **Purpose:** Allows future agents to align immediately.

4.  **DEVELOPMENT STANDARDS:**
    *   Setup commands (`git clone` -> `npm install`).
    *   Scripts table.
    *   Principles (SOLID, DRY, YAGNI).

--- 

## 6. CHAIN OF THOUGHT (CoT) PROTOCOL
Before generating JSON, perform deep analysis in `<thinking>` block:
1.  **Audit:** Analyze repo content and purpose.
2.  **Pivot/Archive Decision:** Is it junk? If so, rename to `Archived-...`. If not, PIVOT to elite status.
3.  **Naming Strategy:** Apply `<Product>-<Function>-<Type>` formula.
4.  **Replication Protocol:** Draft the "AI Agent Directives" block.
5.  **File Generation:** Plan the content for all 11 required files (including `PROPOSED_README.md` and `badges.yml`).
6.  **Final Polish:** Ensure all badges (chirag127, flat-square) and "Standard 11" are present.
7.  **Strict Adherence:** Ensure `PROPOSED_README.md` strictly follows the `AGENTS.md` directives.

--- 

## 7. DYNAMIC URL & BADGE PROTOCOL
**Mandate:** All generated files MUST use the correct dynamic URLs based on the **New Repository Name**.

**Rules:**
1.  **Base URL:** `https://github.com/chirag127/<New-Repo-Name>`
2.  **Badge URLs:** All badges (Shields.io) must point to this Base URL or its specific workflows (e.g., `/actions/workflows/ci.yml`).
3.  **Consistency:** Never use the old/original repository name in links. Always use the new "Apex" name.
4.  **AGENTS.md Customization:** The generated `AGENTS.md` **MUST** be customized for the specific repository's technology stack (e.g., if Rust, use Rust tools; if Python, use Python tools), while retaining the core Apex principles. Do not just copy the generic template; adapt it.

--- 

</details>

## Contributing

Contributions are welcome! Please refer to the [CONTRIBUTING.md](https://github.com/chirag127/CogniTask-AI-Powered-Workflow-Automation-Engine-Python/blob/main/.github/CONTRIBUTING.md) file for detailed guidelines.

## License

This project is licensed under the Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0) - see the [LICENSE](https://github.com/chirag127/CogniTask-AI-Powered-Workflow-Automation-Engine-Python/blob/main/LICENSE) file for details.

## Security

For security-related issues, please refer to the [SECURITY.md](https://github.com/chirag127/CogniTask-AI-Powered-Workflow-Automation-Engine-Python/blob/main/.github/SECURITY.md) file.

[Back to Top](#cognitask-ai-powered-workflow-automation-engine-python)

---
# CogniTask: AI-Powered Workflow Automation Engine (Python)

A sophisticated, modular Python framework leveraging LLMs for complex, multi-step task automation and personal workflow orchestration.

[![Build Status](https://img.shields.io/github/actions/workflow/user/chirag127/CogniTask-AI-Powered-Workflow-Automation-Engine-Python/ci.yml?style=flat-square&logo=githubactions)](https://github.com/chirag127/CogniTask-AI-Powered-Workflow-Automation-Engine-Python/actions/workflows/ci.yml)
[![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/CogniTask-AI-Powered-Workflow-Automation-Engine-Python?style=flat-square&logo=codecov)](https://codecov.io/gh/chirag127/CogniTask-AI-Powered-Workflow-Automation-Engine-Python)
[![Python Version](https://img.shields.io/badge/python-3.10+-blue.svg?style=flat-square&logo=python)](https://www.python.org/)
[![Ruff Lint](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/static/badge.json&style=flat-square&logo=ruff)](https://github.com/charliermarsh/ruff)
[![License](https://img.shields.io/github/license/chirag127/CogniTask-AI-Powered-Workflow-Automation-Engine-Python?style=flat-square&logo=creativecommons)](https://github.com/chirag127/CogniTask-AI-Powered-Workflow-Automation-Engine-Python/blob/main/LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/CogniTask-AI-Powered-Workflow-Automation-Engine-Python?style=flat-square&logo=github)](https://github.com/chirag127/CogniTask-AI-Powered-Workflow-Automation-Engine-Python)

## ✨ Vision

Empower individuals and teams to automate complex, multi-step workflows using the intelligence of Large Language Models (LLMs), making sophisticated task orchestration accessible via a modular Python framework.

## 🚀 Architecture Overview

This project follows a **Modular Monolith** architectural pattern. This approach balances the benefits of modularity (separation of concerns, testability) with the simplicity of a single deployment unit. Key components are isolated into distinct modules, allowing for clear boundaries and easier maintenance.

mermaid
graph TD
    A[CLI Interface] --> B{Orchestration Engine}
    B --> C(AI Module - LLM Integration)
    B --> D(GitHub API Module)
    B --> E(Task Execution Module)
    E --> F(External Services/APIs)
    C --> G[LLM Provider API]
    D --> H[GitHub API]


## 📜 Table of Contents

*   [CogniTask: AI-Powered Workflow Automation Engine (Python)](#cognitask-ai-powered-workflow-automation-engine-python)
*   [Vision](#vision)
*   [Architecture Overview](#architecture-overview)
*   [Table of Contents](#table-of-contents)
*   [AI Agent Directives](#ai-agent-directives)
*   [Key Technologies](#key-technologies)
*   [Development Setup](#development-setup)
*   [Project Structure](#project-structure)
*   [Core Principles](#core-principles)
*   [Contributing](#contributing)
*   [License](#license)

<details>
<summary>🤖 AI AGENT DIRECTIVES (DECEMBER 2025 EDITION)</summary>

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
*   **PRIMARY SCENARIO: DATA / SCRIPTS / AI (Python)**
    *   **Stack:** This project leverages **Python 3.10+**. Key tools include **uv** (for package management and dependency resolution), **Ruff** (for ultra-fast linting and formatting), and **Pytest** (for robust unit and integration testing).
    *   **Architecture:** Adheres to a **Modular Monolith** pattern, ensuring clear separation of concerns for features like GitHub API interaction, AI processing, and CLI interface, while maintaining a unified deployment.
    *   **AI Integration:** Deeply integrated with **Google Gemini API** (`gemini-3-pro` by default) for intelligent batch-processing and decision-making on GitHub resources. Prioritize modular design, clear API contracts, and robust error handling for all AI model interactions.
    *   **CLI Framework:** Uses `Click` or similar for a powerful and intuitive command-line interface.

*   **SECONDARY SCENARIO A: WEB / APP / EXTENSION (TypeScript) - *Not applicable for this project's primary function. Reference only for potential future web-based extensions.***
    *   **Stack:** TypeScript 6.x (Strict), Vite 7 (Rolldown), Tauri v2.x (Native), WXT (Extensions).
    *   **State:** Signals (Standardized).

--- 

## 4. REPOSITORY MANAGEMENT PROTOCOL
*   **METADATA PRECISION:** Name, Description, and Topics must be accurate, professional, and keyword-rich for discoverability.
*   **VERSIONING STANDARD:** Adhere to Semantic Versioning (SemVer) rigorously.
*   **SECURITY FIRST:** All dependencies must be scanned for vulnerabilities. Sensitive data must NOT be committed. Implement robust input validation and output encoding.

--- 

## 5. TESTING AND VERIFICATION MANDATE
*   **TESTING PYRAMID:** Emphasize unit tests, followed by integration tests, and finally, end-to-end tests where applicable.
*   **TESTING FRAMEWORK:** Utilize **Pytest** for all testing needs.
*   **MOCKING STRATEGY:** Employ `unittest.mock` or similar libraries for isolating dependencies during unit testing.
*   **COVERAGE TARGET:** Maintain a minimum of **85% code coverage**. Run coverage reports regularly.
*   **VERIFICATION COMMANDS:**
    *   **Linting & Formatting:** `uv run ruff check . --fix`
    *   **Type Checking:** `uv run mypy .`
    *   **Unit Tests:** `uv run pytest ./tests/unit --cov=cognitask --cov-report=xml`
    *   **Integration Tests:** `uv run pytest ./tests/integration`
    *   **Full Test Suite:** `uv run pytest --cov=cognitask --cov-report=xml`

--- 

## 6. CODE QUALITY AND ARCHITECTURE STANDARDS
*   **PRINCIPLES:** Adhere strictly to SOLID, DRY, KISS, and YAGNI principles.
*   **MODULAR DESIGN:** Favor composition over inheritance. Ensure modules have clear responsibilities and minimal coupling.
*   **ERROR HANDLING:** Implement comprehensive try-except blocks. Define custom exception types where appropriate. Ensure graceful failure and informative error messages.
*   **LLM INTEGRATION:** Design AI interactions with idempotency in mind. Implement retries with exponential backoff for API calls. Cache LLM responses where feasible.
*   **SECRET MANAGEMENT:** Utilize environment variables or a dedicated secrets management tool (e.g., `python-dotenv`, HashiCorp Vault) for sensitive information. NEVER hardcode secrets.

--- 

## 7. DOCUMENTATION AND READABILITY
*   **DOCSTRINGS:** All public functions, classes, and modules must have clear, concise docstrings following the Google or NumPy style guide.
*   **README:** Maintain a comprehensive `README.md` as the project's primary interface.
*   **TYPE HINTS:** Utilize Python's type hinting extensively for improved code clarity and static analysis.

--- 

## 8. DEPLOYMENT AND CI/CD
*   **CI/CD PIPELINE:** Automate testing, linting, and building using GitHub Actions (`.github/workflows/ci.yml`).
*   **PACKAGE MANAGEMENT:** Use `uv` for dependency management. Publish packages to PyPI using a standardized workflow.
*   **CONTAINERIZATION (Optional):** Consider Docker for consistent development and deployment environments.

</details>

## 🚀 Key Technologies

*   **Language:** Python 3.10+
*   **Package Management:** `uv`
*   **Linting & Formatting:** `Ruff`
*   **Testing:** `Pytest`
*   **AI Integration:** Google Gemini API (via `google-generativeai` SDK)
*   **CLI Framework:** `Click`
*   **Architecture:** Modular Monolith

## 💾 Development Setup

1.  **Clone the Repository:**
    bash
    git clone https://github.com/chirag127/CogniTask-AI-Powered-Workflow-Automation-Engine-Python.git
    cd CogniTask-AI-Powered-Workflow-Automation-Engine-Python
    

2.  **Set up Virtual Environment & Install Dependencies:**
    bash
    # Using uv for environment and dependency management
    uv venv
    uv activate
    uv sync
    

3.  **Set Environment Variables:**
    Create a `.env` file in the root directory:
    ini
    # Example .env file
    GEMINI_API_KEY=YOUR_GEMINI_API_KEY
    # Add other necessary environment variables here
    

4.  **Run Linters and Formatters:**
    bash
    uv run ruff check .
    uv run ruff format .
    

5.  **Run Tests:**
    bash
    uv run pytest
    

## 📁 Project Structure


CogniTask-AI-Powered-Workflow-Automation-Engine-Python/
├── .github/
│   ├── workflows/
│   │   └── ci.yml
│   ├── ISSUE_TEMPLATE/
│   │   └── bug_report.md
│   ├── PULL_REQUEST_TEMPLATE.md
│   └── SECURITY.md
├── cognitask/
│   ├── __init__.py
│   ├── cli.py              # CLI entry point
│   ├── core/
│   │   ├── __init__.py
│   │   ├── orchestrator.py # Main workflow logic
│   │   └── task_runner.py  # Executes individual tasks
│   ├── ai/
│   │   ├── __init__.py
│   │   └── llm_service.py  # Interface with LLM APIs (e.g., Gemini)
│   ├── integrations/
│   │   ├── __init__.py
│   │   └── github_api.py   # GitHub API interaction module
│   └── utils/
│       ├── __init__.py
│       └── helpers.py      # Utility functions
├── tests/
│   ├── __init__.py
│   ├── unit/
│   │   └── test_llm_service.py
│   └── integration/
│       └── test_orchestrator.py
├── .env.example
├── .gitignore
├── AGENTS.md
├── badges.yml
├── LICENSE
├── pyproject.toml        # Project metadata and uv/ruff configuration
├── README.md
└── setup.py              # Legacy setup script (if needed)


## 💡 Core Principles

*   **SOLID:** Ensuring maintainable and scalable object-oriented design.
*   **DRY (Don't Repeat Yourself):** Minimizing redundant code.
*   **KISS (Keep It Simple, Stupid):** Favoring straightforward solutions.
*   **YAGNI (You Ain't Gonna Need It):** Avoiding unnecessary complexity and features.
*   **Modularity:** Designing independent, reusable components.
*   **Automation First:** Automating workflows and development processes.

## 🤝 Contributing

Contributions are welcome! Please follow the guidelines in `CONTRIBUTING.md`.

## 📜 License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0)**. See the `LICENSE` file for more details.

--- 

*Star ⭐ this Repo if you find it useful!*
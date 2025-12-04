# Contributing to CogniTask-AI-Powered-Workflow-Automation-Engine-Python

We welcome contributions to `CogniTask-AI-Powered-Workflow-Automation-Engine-Python`! To ensure a high-quality, consistent, and professional project, please adhere to the following guidelines.

## 1. Code of Conduct

This project adheres to the Contributor Covenant Code of Conduct v2.1. For more details, please see our [CODE_OF_CONDUCT.md](https://github.com/chirag127/CogniTask-AI-Powered-Workflow-Automation-Engine-Python/blob/main/CODE_OF_CONDUCT.md).

## 2. Getting Started

### Prerequisites

*   **Python:** Version 3.10+ is required.
*   **uv:** The project uses `uv` for package management. Ensure you have it installed.
*   **Ruff:** For linting and formatting.
*   **Pytest:** For running tests.

### Setup

1.  **Clone the Repository:**
    bash
    git clone https://github.com/chirag127/CogniTask-AI-Powered-Workflow-Automation-Engine-Python.git
    cd CogniTask-AI-Powered-Workflow-Automation-Engine-Python
    

2.  **Install Dependencies:**
    Use `uv` to install project dependencies and development tools.
    bash
    uv venv --python 3.10 # Or your preferred Python version >= 3.10
    uv pip install --editable "[dev]"
    

## 3. Development Workflow

We follow a standard Git workflow:

1.  **Fork the Repository:** Create your own fork of the `chirag127/CogniTask-AI-Powered-Workflow-Automation-Engine-Python` repository.
2.  **Create a Branch:** Start a new branch for your feature or bug fix. Use a descriptive name (e.g., `feature/add-new-llm-adapter`, `fix/resolve-api-rate-limiting`).
    bash
    git checkout -b your-branch-name
    
3.  **Make Changes:** Implement your changes, ensuring they align with the project's architectural principles and coding standards.
4.  **Lint and Format:** Run Ruff to ensure your code adheres to style guidelines.
    bash
    ruff check .
    ruff format .
    
5.  **Run Tests:** Execute all tests using Pytest to verify your changes and ensure no regressions.
    bash
    pytest
    
6.  **Commit Changes:** Commit your changes with clear, concise commit messages.
    bash
    git commit -am "feat: Add concise description for new LLM adapter"
    
7.  **Push Changes:** Push your branch to your fork.
    bash
    git push origin your-branch-name
    
8.  **Open a Pull Request:** Create a Pull Request from your branch on your fork to the `main` branch of the `chirag127/CogniTask-AI-Powered-Workflow-Automation-Engine-Python` repository.

## 4. Pull Request Guidelines

*   **Descriptive Title:** Clearly state the purpose of your PR.
*   **Detailed Description:** Explain the changes, the problem they solve, and any relevant context. Reference any related issues.
*   **Testing:** Ensure all tests pass. If you add new functionality, include new tests.
*   **Code Review:** Be prepared to address feedback from reviewers.
*   **AI Agent Alignment:** Ensure your changes do not conflict with the directives in `AGENTS.md` and that any new AI integrations are modular and well-documented.

## 5. Architectural Principles

This project is built upon the following core principles:

*   **SOLID:** Maintain Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, and Dependency Inversion.
*   **DRY (Don't Repeat Yourself):** Avoid redundant code.
*   **YAGNI (You Ain't Gonna Need It):** Implement only what is necessary for current features.
*   **Modularity:** Favor well-defined modules with clear interfaces, especially for AI integrations and external service interactions.
*   **Pythonic:** Write clean, readable, and idiomatic Python code.

## 6. Reporting Issues

If you encounter a bug or have a feature request:

1.  **Search Existing Issues:** Check if a similar issue has already been reported.
2.  **Create a New Issue:** If not, create a new issue using the provided templates (`.github/ISSUE_TEMPLATE/bug_report.md`).
3.  **Provide Details:** Include a clear description, steps to reproduce, expected vs. actual behavior, environment details (Python version, OS), and any relevant logs or screenshots.

## 7. Thank You!

Thank you for contributing to `CogniTask-AI-Powered-Workflow-Automation-Engine-Python`. Your efforts help make this project better for everyone.

# Security Policy

## Supported Versions

| Version | Supported          |
| ------- | ------------------ |
| 3.10.x  | :white_check_mark: |
| 3.11.x  | :white_check_mark: |
| 3.12.x  | :white_check_mark: |
| 3.13.x  | :white_check_mark: |


## Reporting a Vulnerability

We take security seriously. If you find a security vulnerability in `CogniTask-AI-Powered-Workflow-Automation-Engine-Python`, please report it to us by following these steps:

1.  **DO NOT** open a public issue. Please use the GitHub Security Advisory feature.
2.  Go to `https://github.com/chirag127/CogniTask-AI-Powered-Workflow-Automation-Engine-Python/security/advisories/new`.
3.  Provide a detailed description of the vulnerability, including:
    *   The affected version(s).
    *   Steps to reproduce the vulnerability.
    *   Potential impact.
    *   Any relevant code snippets or configurations.
4.  If you have discovered a vulnerability that you believe is critical and requires immediate attention, or if you are unsure how to use the Security Advisory feature, please contact the maintainers directly at [security@example.com](mailto:security@example.com) (Please note: This is a placeholder email. Real security vulnerabilities should be reported via GitHub Security Advisories).

We will acknowledge your report promptly and will work to address the issue as quickly as possible. We will also communicate the release of any fixes or mitigations via security advisories.

## Responsible Disclosure

We will NOT take legal action against individuals who report security vulnerabilities in good faith, provided they adhere to the following:

*   They give us adequate time to fix the vulnerability before making any information public.
*   They do not disrupt our services or access/modify/delete data beyond what is necessary to demonstrate the vulnerability.
*   They do not exploit the vulnerability to compromise the data of other users.
*   They do not social engineer, phishing, or conduct any other malicious activity against our users or employees.

If you find a vulnerability, please report it following the steps above. Thank you for helping keep `CogniTask-AI-Powered-Workflow-Automation-Engine-Python` secure.

## Security Tools & Practices

This project employs several security-focused tools and practices:

*   **Dependency Scanning:** Automated scans for known vulnerabilities in dependencies using tools integrated into GitHub Actions.
*   **Linting & Formatting:** Strict enforcement of code style and potential error detection using **Ruff** to maintain code quality and reduce surface area for bugs.
*   **Testing:** Comprehensive unit and integration tests using **Pytest** to catch regressions and ensure predictable behavior.
*   **AI Model Security:** Careful consideration of prompt injection, data privacy, and model output validation when interacting with LLMs, particularly the Google Gemini API.
*   **Secure Development Lifecycle:** Adherence to principles of secure coding, minimizing attack vectors, and validating all inputs.

For more detailed information on our development standards, please refer to the `AGENTS.md` file within this repository.

---
name: Bug Report
about: Report a bug in the CogniTask project
title: "Bug: "
labels: "bug"
assignees:

body:
  - type: markdown
    attributes:
      value: |+
        ## Bug Report Template

        Thank you for taking the time to report a bug! Please provide as much detail as possible to help us diagnose and fix the issue.

        **Before reporting:**
        *   Please check if the issue has already been reported.
        *   Ensure you are using the latest version of the `CogniTask-AI-Powered-Workflow-Automation-Engine-Python`.

        **Project Repository:** https://github.com/chirag127/CogniTask-AI-Powered-Workflow-Automation-Engine-Python

  - type: input
    id: version
    attributes:
      label: Version of CogniTask
      description: Please specify the version of the CogniTask you are experiencing this bug with.
      placeholder: e.g., 1.2.0
    validations:
      required: true
  - type: input
    id: os
    attributes:
      label: Operating System & Version
      description: e.g., Windows 11, macOS Ventura 13.6, Ubuntu 22.04
      placeholder: e.g., macOS Ventura 13.6
    validations:
      required: true
  - type: input
    id: python-version
    attributes:
      label: Python Version
      description: e.g., Python 3.11.5
      placeholder: e.g., Python 3.11.5
    validations:
      required: true
  - type: textarea
    id: description
    attributes:
      label: Description of the bug
      description: A clear and concise description of what the bug is.
      placeholder: |-
        What is the unexpected behavior?
        What did you expect to happen?
    validations:
      required: true
  - type: textarea
    id: steps_to_reproduce
    attributes:
      label: Steps to Reproduce
      description: Provide a step-by-step guide to reproduce the bug.
      placeholder: |-
        1. Go to '...' location
        2. Click on '....'
        3. Scroll down '....'
        4. See error
    validations:
      required: true
  - type: textarea
    id: expected_behavior
    attributes:
      label: Expected Behavior
      description: Describe what you expected to happen.
      placeholder: |-
        I expected X to happen, but Y occurred.
    validations:
      required: false
  - type: textarea
    id: actual_behavior
    attributes:
      label: Actual Behavior
      description: Describe what actually happened.
      placeholder: |-
        Instead of X, Y happened.
    validations:
      required: false
  - type: textarea
    id: logs
    attributes:
      label: Relevant Logs (if applicable)
      description: Please paste any relevant error messages or logs from the console or application output. Use code blocks for formatting.
      placeholder: |-
        
        [Error message or log output here]
        
    validations:
      required: false
  - type: textarea
    id: additional_context
    attributes:
      label: Additional Context
      description: Provide any other information that might be helpful, such as screenshots, configuration files, or scenarios where the bug occurs.
      placeholder: |-
        Screenshots, relevant configuration snippets, user workflow details, etc.
    validations:
      required: false
  - type: markdown
    attributes:
      value: |+
        ---

name: Bug Report
about: Report a bug or unexpected behavior in TOTPBOX
title: "[BUG] "
labels: ["bug", "needs-triage"]
assignees: []

body:
  - type: markdown
    attributes:
      value: |
        Thanks for taking the time to report a bug! Please fill in as much detail as possible.

  - type: textarea
    id: description
    attributes:
      label: Bug Description
      description: A clear and concise description of what the bug is.
      placeholder: Describe the bug...
    validations:
      required: true

  - type: textarea
    id: steps
    attributes:
      label: Steps to Reproduce
      description: Step-by-step instructions to reproduce the behavior.
      placeholder: |
        1. Go to '...'
        2. Call '...'
        3. See error
    validations:
      required: true

  - type: textarea
    id: expected
    attributes:
      label: Expected Behavior
      description: What did you expect to happen?
    validations:
      required: true

  - type: textarea
    id: actual
    attributes:
      label: Actual Behavior
      description: What actually happened?
    validations:
      required: true

  - type: input
    id: version
    attributes:
      label: TOTPBOX Version
      placeholder: e.g. 1.2.3
    validations:
      required: false

  - type: dropdown
    id: platform
    attributes:
      label: Platform
      options:
        - Web
        - iOS
        - Android
        - API / SDK
        - Other
    validations:
      required: false

  - type: textarea
    id: context
    attributes:
      label: Additional Context
      description: Any other context, screenshots, or logs.
    validations:
      required: false

  - type: checkboxes
    id: confirmation
    attributes:
      label: Checklist
      options:
        - label: I have searched existing issues to avoid duplicates
          required: true
        - label: I am not reporting a security vulnerability (see SECURITY.md for that)
          required: true

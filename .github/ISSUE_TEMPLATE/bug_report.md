---
name: Bug Report
about: Report a bug in a Label Studio configuration
title: "[BUG] "
labels: bug
assignees: ''
body:
  - type: markdown
    attributes:
      value: |
        Thanks for reporting a bug in our Label Studio configurations collection!
                
  - type: input
    id: config-name
    attributes:
      label: Label Config Name
      description: Which label config has the issue?
      placeholder: e.g., html-ner-tagging
    validations:
      required: false
      
  - type: textarea
    id: bug-description
    attributes:
      label: What's the bug?
      description: Clear description of what's not working correctly
      placeholder: The labels aren't showing properly when...
    validations:
      required: true
      
  - type: textarea
    id: reproduction
    attributes:
      label: Steps to reproduce
      description: How can we see this bug?
      placeholder: |
        1. Import this config
        2. Load sample data
        3. Try to label X
        4. See error
    validations:
      required: true
      
  - type: textarea
    id: expected-behavior
    attributes:
      label: Expected behavior
      description: What should happen instead?
      placeholder: The labels should appear correctly when...
    validations:
      required: true
      
  - type: textarea
    id: screenshots
    attributes:
      label: Screenshots/Logs
      description: Images or logs that show the problem
      placeholder: Paste or drag images here
    validations:
      required: false
      
  - type: input
    id: label-studio-version
    attributes:
      label: Label Studio Version
      description: Which Label Studio version are you using?
      placeholder: e.g., 1.8.0
    validations:
      required: false
      
  - type: dropdown
    id: edition
    attributes:
      label: Label Studio Edition
      description: Which edition of Label Studio are you using?
      options:
        - Open Source Community Edition
        - Enterprise Edition
        - Not sure
    validations:
      required: false
---
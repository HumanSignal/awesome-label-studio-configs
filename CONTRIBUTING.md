# Contributing to Awesome Label Studio Configs

We love your input! Help us improve and grow.

## Getting Started

1. **Fork** this repository on GitHub.
2. **Clone** your fork and create a new branch (e.g., `git checkout -b feature/my-config`).
3. Add or update label configs, sample data, or documentation.
4. **Test** your changes locally or with Label Studio.
5. **Open a Pull Request** and fill out the template to describe your changes.

## Contributing Label Configs

### Adding a New Label Config

Create a subfolder under `label-configs/` with a clear name (e.g. `label-configs/my-cool-config`).
Add the following required files:

1. **A label config file** (XML or JSON)
2. **Sample data** (e.g., tasks in JSON)
3. **A README** that describes how to use it
4. **A `preview/` folder** with screenshots/GIFs
5. **A manifest.json file** with metadata about your config

The manifest follows our JSON schema which will be validated during checks.

### Updating an Existing Label Config

If you're improving an existing config:

1. **Add yourself as a contributor** in the manifest.json file by adding your GitHub username to the "contributors" array
2. **Update the version number** following semantic versioning:
   - Increment MAJOR version for incompatible changes
   - Increment MINOR version for new functionality in a backward compatible manner
   - Increment PATCH version for backward compatible bug fixes
3. **Update screenshots** if your changes affect the UI appearance
4. **Explain your changes** in the PR description, including why they improve the config
5. **Ensure all validation checks pass** before submitting your PR

## Validation and Checks

Two layers of validation ensure your contributions meet our quality standards:

### 1. Local Pre-Push Hooks

All validation happens automatically during git push when pre-commit hooks are set up. The checks include:

- Basic syntax validation for XML, JSON, and YAML files
- JSON Schema validation on manifest.json files
- Directory structure validation (required files and naming conventions)
- Checks for the presence of a preview folder with screenshots

**Note:** The first time you push, pre-commit will show "Initializing environment" messages and may take
a few minutes to set up. This is normal and subsequent runs will be much faster.

### 2. GitHub Actions CI

When you create a pull request, GitHub Actions will automatically run the same validations.
This ensures that all contributions meet the requirements even if you didn't set up the pre-commit hooks locally.

## Reviewing Pull Requests

- Make sure your PR passes all automated checks.
- A maintainer will review your changes and merge them once approved.

Thank you for making this project better!

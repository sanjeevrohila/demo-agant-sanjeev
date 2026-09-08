# Contributing Guidelines

Thank you for considering contributing to this project! We welcome contributions of all kinds, from bug reports and feature requests to pull requests with code improvements. Please follow these guidelines to make the contribution process smooth for everyone.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How to Contribute](#how-to-contribute)
  - [Reporting Bugs](#reporting-bugs)
  - [Suggesting Enhancements](#suggesting-enhancements)
  - [Submitting Pull Requests](#submitting-pull-requests)
- [Development Setup](#development-setup)
- [Style Guidelines](#style-guidelines)
- [Testing](#testing)
- [Documentation Updates](#documentation-updates)
- [Commit Message Format](#commit-message-format)
- [License](#license)

## Code of Conduct

Please note that this project adheres to a [Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code.

## How to Contribute

### Reporting Bugs

1. **Search existing issues** to see if the bug has already been reported.
2. If not, open a **new issue** with:
   - A clear title.
   - A description of the problem.
   - Steps to reproduce the bug.
   - Expected vs. actual behavior.
   - Environment details (OS, Python version, etc.).

### Suggesting Enhancements

1. Check the issue tracker for similar ideas.
2. Open a **new issue** titled with a concise description of the enhancement.
3. Provide a detailed explanation of why the change is beneficial, and any potential drawbacks.

### Submitting Pull Requests

1. **Fork** the repository and **clone** your fork locally.
2. **Create a new branch** for your work:
   ```bash
   git checkout -b my-feature-branch
   ```
3. Make your changes, ensuring they follow the style guidelines (see below).
4. **Write tests** for new functionality or bug fixes.
5. Run the test suite to ensure everything passes:
   ```bash
   pytest
   ```
6. **Commit** your changes with a clear, descriptive commit message (see Commit Message Format).
7. Push your branch to your fork:
   ```bash
   git push origin my-feature-branch
   ```
8. Open a **pull request** against the `main` branch of the original repository.
   - Include a description of what the PR does.
   - Reference any related issues using `#issue-number`.
   - Ensure the CI checks pass.

## Development Setup

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-org/your-repo.git
   cd your-repo
   ```
2. **Create a virtual environment** and install dependencies:
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows use `venv\Scripts\activate`
   pip install -r requirements.txt
   ```
3. Install development dependencies (testing, linting, etc.) if they are listed in `requirements-dev.txt`:
   ```bash
   pip install -r requirements-dev.txt
   ```

## Style Guidelines

- Follow the project's existing coding style (PEP 8 for Python).
- Use **black** for formatting and **flake8** for linting.
- Keep line length to 88 characters where possible.
- Use descriptive variable and function names.

## Testing

- Write unit tests for any new code using **pytest**.
- Place tests in the `tests/` directory mirroring the package structure.
- Aim for high coverage; run coverage reports with:
  ```bash
  pytest --cov=your_package
  ```

## Documentation Updates

- Update the relevant docstrings and markdown files when you add or change functionality.
- If you add a new public API, ensure it is documented in the appropriate module README or the central documentation site.

## Commit Message Format

Use a clear, concise commit message format:

```
<type>(<scope>): <subject>

<body>

<footer>
```

- **type**: `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`
- **scope** (optional): the area of code affected, e.g., `parser`, `cli`
- **subject**: short description (max 50 characters)
- **body** (optional): detailed explanation, why and how
- **footer** (optional): references to issues, breaking changes, etc.

Example:
```
feat(parser): add support for JSON input

The parser now accepts JSON files in addition to the existing XML format.
Closes #42.
```

## License

By contributing, you agree that your contributions will be licensed under the project's [MIT License](LICENSE).

---

We appreciate your help in making this project better! 🎉
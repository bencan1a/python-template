# Python Template 🐍

A comprehensive Python project template optimized for GitHub Copilot and modern development practices.

[![CI](https://github.com/bencan1a/python-template/workflows/CI/badge.svg)](https://github.com/bencan1a/python-template/actions)
[![Python Version](https://img.shields.io/badge/python-3.10%2B-blue)](https://www.python.org/downloads/)
[![Code style: ruff](https://img.shields.io/badge/code%20style-ruff-000000.svg)](https://github.com/astral-sh/ruff)
[![Type checked: mypy](https://img.shields.io/badge/type%20checked-mypy-blue)](http://mypy-lang.org/)
[![Security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)

## ✨ Features

This template includes everything you need to start a professional Python project:

- 🏗️ **Modern Project Structure**: Standard `src/` layout following Python best practices
- 🛠️ **Development Container**: Pre-configured devcontainer with all necessary tools
- 🔍 **Code Quality Tools**: Ruff, Black, mypy, and Bandit pre-installed and configured
- 🧪 **Testing Setup**: pytest with coverage reporting and example tests
- 🤖 **GitHub Actions**: CI/CD workflows for validation, PR checks, and nightly regression
- 📝 **Documentation Ready**: Structured for easy documentation generation
- 🎯 **Custom Agent Profiles**: Specialized GitHub Copilot agent configurations
- ⚙️ **Editor Configuration**: .editorconfig and .gitattributes for consistency
- 📋 **Pull Request Template**: Comprehensive PR template for quality reviews

## 🚀 Quick Start

### Prerequisites

- Python 3.10 or higher
- pip or uv package manager
- Git

### Installation

1. **Use this template**: Click "Use this template" button on GitHub

2. **Clone your new repository**:
   ```bash
   git clone https://github.com/yourusername/your-project-name.git
   cd your-project-name
   ```

3. **Install dependencies**:
   ```bash
   pip install -e '.[dev]'
   ```

4. **Set up pre-commit hooks** (optional but recommended):
   ```bash
   pre-commit install
   ```

### Using DevContainer (Recommended)

Open the project in Visual Studio Code and reopen in container when prompted. All dependencies will be automatically installed.

## 📖 Usage

### Running Tests

```bash
# Run all tests
pytest

# Run with coverage
pytest --cov=src

# Run specific test file
pytest tests/test_calculator.py

# Run tests matching a pattern
pytest -k "test_add"
```

### Code Quality Checks

```bash
# Format code
ruff format .

# Lint code
ruff check .

# Type check
mypy .

# Security scan
bandit -r src/
```

### Running All Checks (pre-commit)

```bash
pre-commit run --all-files
```

## 🗂️ Project Structure

```
.
├── .devcontainer/          # Development container configuration
├── .github/
│   ├── agents/            # Custom GitHub Copilot agent profiles
│   ├── workflows/         # GitHub Actions workflows
│   └── pull_request_template.md
├── src/
│   └── python_template/   # Main package source code
│       ├── __init__.py
│       ├── calculator.py
│       └── greeter.py
├── tests/                 # Test files
│   ├── conftest.py
│   ├── test_calculator.py
│   └── test_greeter.py
├── .editorconfig          # Editor configuration
├── .gitattributes         # Git attributes for consistent line endings
├── .gitignore            # Git ignore patterns
├── .pre-commit-config.yaml # Pre-commit hooks configuration
├── pyproject.toml        # Project configuration and dependencies
├── LICENSE               # License file
└── README.md            # This file
```

## 🤖 GitHub Copilot Agent Profiles

This template includes specialized agent profiles in `.github/agents/`:

- **Architecture Agent**: System design and architectural decisions
- **Test Agent**: Test writing and testing strategies
- **Debug Agent**: Debugging and troubleshooting
- **Documentation Agent**: Technical writing and documentation

See [.github/agents/README.md](.github/agents/README.md) for detailed usage instructions.

## 🔧 Configuration

### Customizing for Your Project

1. **Update `pyproject.toml`**:
   - Change `name`, `description`, `authors`
   - Add your specific dependencies
   - Adjust tool configurations as needed

2. **Update package name**:
   - Rename `src/python_template/` to your package name
   - Update imports in `__init__.py` and tests

3. **Configure GitHub Actions**:
   - Review workflows in `.github/workflows/`
   - Adjust Python versions, OS matrices as needed
   - Add secrets for deployment if required

4. **Update README**:
   - Replace this content with your project documentation
   - Update badges with your repository information

## 🧰 Pre-installed Tools

### Code Quality
- **Ruff**: Fast Python linter and formatter
- **Black**: Code formatter (alternative to ruff format)
- **mypy**: Static type checker
- **Bandit**: Security vulnerability scanner

### Testing
- **pytest**: Testing framework
- **pytest-cov**: Coverage plugin
- **pytest-asyncio**: Async test support
- **pytest-mock**: Mocking support
- **hypothesis**: Property-based testing
- **faker**: Test data generation

### Development
- **pre-commit**: Git hooks framework
- **ipython**: Enhanced Python shell
- **ipdb**: IPython debugger

## 📊 GitHub Actions Workflows

### CI Workflow (`ci.yml`)
Runs on push and pull requests:
- Lint and format checking
- Type checking with mypy
- Security scanning with bandit
- Tests across multiple OS and Python versions
- Coverage reporting

### PR Workflow (`pr.yml`)
Runs on pull requests:
- Validates all code quality checks
- Posts summary comment on PR
- Checks for breaking changes

### Nightly Regression (`nightly.yml`)
Runs daily at 2 AM UTC:
- Full test suite across all platforms
- Performance testing
- Dependency security audit
- Creates issue on failure

## 🤝 Contributing

1. Create a feature branch
2. Make your changes
3. Run tests and quality checks
4. Submit a pull request

All pull requests must:
- Pass all CI checks
- Include tests for new functionality
- Follow the project's code style
- Include documentation updates if needed

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built with modern Python best practices
- Optimized for GitHub Copilot workflow
- Inspired by the Python community's excellent tooling

## 📚 Resources

- [Python Packaging Guide](https://packaging.python.org/)
- [pytest Documentation](https://docs.pytest.org/)
- [Ruff Documentation](https://docs.astral.sh/ruff/)
- [mypy Documentation](https://mypy.readthedocs.io/)
- [GitHub Copilot Documentation](https://docs.github.com/copilot)

---

**Happy Coding! 🎉**

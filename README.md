# marimo + Poetry Starter Template

A starter template for [marimo](https://marimo.io) notebooks using [Poetry](https://python-poetry.org) for dependency and project management. This template provides a modern Python development setup with best practices for notebook development.

## Features

- 🚀 Python 3.12+ support
- 📦 Dependency management with Poetry
- 🧪 Testing setup with pytest
- 🎯 Code quality with Ruff (linting + formatting)
- 👷 CI/CD with GitHub Actions
- 📓 Interactive notebook development with marimo

## Prerequisites

- Python 3.12 or higher
- [Poetry](https://python-poetry.org/docs/#installation) installed

## Getting Started

1. Clone this repository:

   ```bash
   git clone https://github.com/yourusername/marimo-poetry-starter-template
   cd marimo-poetry-starter-template
   ```

2. Install dependencies:

   ```bash
   poetry install
   ```

3. Run the marimo editor:

   ```bash
   poetry run marimo edit
   ```

## Development

### Running Tests

```bash
# Run testing in your regular python files
poetry run pytest tests
# Running testing in your marimo notebooks
poetry run pytest src
```

### Linting and formatting

```bash
poetry run ruff check .
poetry run ruff format .
```

### Pre-commit hooks

```bash
poetry run pre-commit install
poetry run pre-commit run --all-files
```

## Project Structure

```markdown
├── .github/            # GitHub Actions workflows
├── src/               # Source code
│   ├── app.py        # Sample marimo notebook
│   └── utils.py      # Utility functions
├── tests/            # Test files
├── pyproject.toml    # Project configuration
└── poetry.lock       # Dependency lock file
```

## License

MIT

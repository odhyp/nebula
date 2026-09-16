<!-- rumdl-disable-file MD013 -->

# Nebula

Nebula is a Python starter template using `uv` for package manager, `ruff` for linting/formatting, and `pre-commit` for Git hook automation.

## Installation

Make sure to have [uv](https://github.com/astral-sh/uv) installed on your machine.

1. Click "[Use this template](https://github.com/odhyp/nebula/generate)" to create a new repository

2. Clone your new repository:

   ```bash
   git clone https://github.com/your-username/project-name.git
   cd project-name
   ```

3. Rename `src/nebula` to `src/project_name`

4. Change `name = "nebula"` to `name = "project-name"` in `pyproject.toml`

5. Initialize the project:

   ```bash
   uv sync
   uv run pre-commit install
   ```

6. Commit changes (automatically linter-checked & formatted)

## Scripts

- Run linter and formatter

  ```bash
  uv run ruff check . --fix
  uv run ruff format .
  ```

- Trigger pre-commit manually across all files:

  ```bash
  uv run pre-commit run --all-files
  ```

# Template for Setting Up a Python Development Environment with VS Devcontainer

## Overview

This repository is a template for setting up a Python development environment using Visual Studio Code's Devcontainer.  
Package management is done using [poetry](https://python-poetry.org/).  
Additionally, [ruff](https://docs.astral.sh/ruff/) is used as the formatter.

## Configuration of python.analysis.extraPaths

1. Execute `poetry env info` and copy the value of `path`.
2. Set the copied value in `.vscode/settings.json` under `python.analysis.extraPaths`. Below is an example configuration.

```json
{
  "python.analysis.extraPaths": [
    "/path/to/poetry/cache/virtualenvs/test-example-py3.10/lib/python3.10/site-packages"
  ]
}
```

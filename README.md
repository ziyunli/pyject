# pyject

[![CI](https://github.com/ziyunli/pyject/actions/workflows/ci.yaml/badge.svg)](https://github.com/ziyunli/pyject/actions/workflows/ci.yaml)

A Python project template. Mostly following setups from https://mitelman.engineering/blog/python-best-practice/automating-python-best-practices-for-a-new-project/.

## Dependencies

* [asdf](https://asdf-vm.com/)
* [poetry](https://poetry.eustace.io/)

## Instructions

First, replace `pyject` in files with your new project name.

And then, run the following commands:

* `poetry install`
* `poetry run pre-commit install`
* `poetry run pre-commit autoupdate`: keep pre-commit config updated to the latest version of tools


Use `poetry shell` to activate the virtual environment.

`poetry run pytest` to run tests.
## How to reproduce

```bash
poetry new {project_name}

cd !$

# with asdf
asdf install python latest
asdf local python latest

# or with pyenv
# pyenv install 3.10.5
# pyenv local 3.10.5

poetry env use python

# Dev toolings
poetry add --dev pytest@latest # poetry new constrained pytest to ^5.2 by default.
poetry add --dev pytest-cov pre-commit flake8 mypy isort black
```

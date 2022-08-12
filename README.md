# pyject

A Python project template following https://mitelman.engineering/blog/python-best-practice/automating-python-best-practices-for-a-new-project/

## Dependencies

* [asdf](https://asdf-vm.com/)
* [poetry](https://poetry.eustace.io/)

## Commands

* `poetry install`
* `poetry shell`
* `pre-commit autoupdate`: keep pre-commit config updated to the latest version of tools


## How to reproduce

```bash
poetry new {project_name}

cd !$

# with pyenv
# pyenv install 3.10.5
pyenv local 3.10.5
poetry env use python

# Dev toolings
poetry add --dev pytest-cov pre-commit flake8 mypy isort black
```

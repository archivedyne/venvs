# Linter and Formatter and Type Checker

Vscode Package

```shell
$ ext install ms-python.python
```

Python Modules:

```shell
$ python3 -m venv .venv
$ source .venv/bin/activate
(.venv) $ pip install flake8 mypy black isort
```

Vscode settings.json:

```json
  // ##########################################
  //                  Python
  // ##########################################
  // Python Venv
   "python.venvPath": ".venv",
   "python.pythonPath": ".venv/bin/python",
  // Python typechecker
  "python.linting.mypyEnabled": true,
  // Python linter
  "python.linting.pylintEnabled": false, // not use pylint
  "python.linting.flake8Enabled": true,
  "python.linting.lintOnSave": true,
  // Python Formatter
  "python.formatting.provider": "black",
  "[python]": {
    "editor.formatOnSave": true,
  }
```

setup.cfg (for top level)

```setup.cfg
[flake8]
max-line-length = 88
ignore = E203,W503,W504

[mypy]
ignore_missing_imports = True
```

## Ref
- https://note.com/10mohi6/n/n87e7867bfb79
- http://flake8.pycqa.org/en/latest/
- https://github.com/python/mypy
- https://github.com/psf/black
- https://medium.com/@marcobelo/setting-up-python-black-on-visual-studio-code-5318eba4cd00

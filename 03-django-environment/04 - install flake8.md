### install flake8

pipenv install flake8 --dev

### create setup.cfg in root of project

setup.cfg

[flake8]
ignore = E203, E266, E501, W503
max-line-length = 88
max-complexity = 18
select = B,C,E,F,W,T4

### add flake to user settings.json vscode

```
"python.linting.flake8Path": "${workspaceFolder}/.venv/bin/flake8",
"python.linting.flake8Enabled": true,
"editor.formatOnSave": true,
```

### ways to run flake8

pipenv run flake8
or
when you complete writing code

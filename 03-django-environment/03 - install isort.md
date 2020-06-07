### install isort extension

command + shift + x ( search isort )

## install isort in env.

pipenv install isort --dev

## create file in root of project

setup.cfg

[isort]
multi_line_output=3
include_trailing_comma=True
force_grid_wrap=0
use_parentheses=True
line_length=88

## ways to run isort

pipenv run isort
or
on everysave

## add below to settings.json on vscode

```
"[python]": {
    "editor.codeActionsOnSave": {
      "source.organizeImports": true
    }
  },
```

### test everything works

paste below into a views.py header and then change values
of setup.cfg e.g line length and see if it picks up

```
  from django.apps import registry
  from django.db import models
  from django.shortcuts import get_object_or_404, redirect, render
```

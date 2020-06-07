## setup environment

https://sourcery.ai/blog/python-best-practices/

### install pipx

pip install --user pipx
pipx ensurepath

### install pipenv

arguement for pipenv: [realpython/pipenv-guide](https://realpython.com/pipenv-guide/)

pipx install pipenv

### start pipenv virtual environment shell

pipenv ( list commands )
pipenv shell
exit
pipenv --rm

### install django

pipenv install django==3.0.6 --dev

### check installed packages

pip list
pip freeze

### install dev specific package

pipenv install pytest --dev

### install packages from Pipfile.lock

pipenv install --ignore-pipfile

### install packages from Pipfile

pipenv install

### view package dependencies

pipenv graph
pipenv graph --reverse

### pipenv open a package

pipenv open flask

### uninstall package

pipenv uninstall [package]

### get path to virtual env

pipenv --venv

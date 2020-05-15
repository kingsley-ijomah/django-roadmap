## Sample Project

### directory structure
`
cd ~/desktop &&
mkdir django-walkthrough &&
cd django-walkthrough &&
mkdir .vscode &&
touch .vscode/settings.json &&
mkdir src
`

---

## create virtual env
> pwd -> django-walkthrough
virtualenv venv

---

## activagte virtual env
source venv/bin/activate

---

## install django into env
pip list
pip install django

---

## start a new project
django-admin startproject code_sample .

---

## start a new app 
python manage.py startapp users

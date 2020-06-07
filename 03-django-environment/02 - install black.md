### select black as default formatter

https://github.com/psf/black
http://www.locallyoptimal.com/blog/2019/08/23/why-you-should-use-black-for-your-python-style-linting/

- CMD + Shift + P
- search user settings: python formatting provider
- select 'black' from droplist

or edit settings.json and add:

"python.formatting.provider": "black"

```
"python.formatting.blackPath": "${workspaceFolder}/.venv/bin/black",
```

### force format on save

add to settings.json: "editor.formatOnSave": true

### now install black into your environment

# sets .venv in current project

PIPENV_VENV_IN_PROJECT=true pipenv shell
pipenv install black --dev

if you get error: missing xcrun at....
then run:
xcode-select --install
or
sudo xcode-select --reset

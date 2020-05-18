## setup visual studio code

Below we are going to configure editor for django

Download the editor:
https://code.visualstudio.com/download

Read about how to use it here:
https://code.visualstudio.com/docs/?dv=osx

---

### install extensions

- click on extension within VSC (visual studio code)
- install python
- install Django Templates and backend snipets
- install Django Template language support
- install Prettier code formatter
- install kite autocomplete
- install Bracket Pair Colorizer
- install Auto Rename Tag
- install CSS Peek
- install HTML CSS Support
- install Live Sass Compiler
- install Live Server
- install Visual Studio Live Share
- install HTML Boilerplate

---

### install kite copilot

read about kite
https://kite.com/

download and install kite copilot and run it
https://kite.com/download/

### set vscode settings.json for user

edit the settings file located below:
~/Library/Application Support/Code/User/settings.json

```
{
  "python.pythonPath": "/Users/kingsley/.pyenv/versions/3.8.0/bin/python",
  "kite.showWelcomeNotificationOnStartup": false,
  "editor.formatOnSave": true,
  "terminal.integrated.fontSize": 14,
  "editor.fontSize": 14,
  "editor.tabSize": 2,
  "python.linting.pycodestyleEnabled": true,
  "python.linting.pylintEnabled": true,
  "python.linting.pylintPath": "pylint",
  "python.linting.pylintArgs": ["--load-plugins", "pylint_django"],
  "python.linting.pydocstyleArgs": ["--ignore=E501"],
  "files.exclude": { "\*\*/\*.pyc": true }
}
```

### read about settings here:

https://code.visualstudio.com/docs/getstarted/settings
https://code.visualstudio.com/docs/python/linting#_enable-linters

### launch VSCode from terminal using `code` keyword

- Launch VS Code.
- Open the Command Palette (⇧⌘P) and type 'shell command'
- Restart the terminal for the new \$PATH value to take effect.

### update .zshrc or .bash_profile

This will make vscode default editor
It also makes it possible to run: pipenv open django

- export EDITOR="code -w"

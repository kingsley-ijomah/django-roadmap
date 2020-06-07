## setup visual studio code

Below we are going to configure editor for django

Download the editor:
https://code.visualstudio.com/download

Read about how to use it here:
https://code.visualstudio.com/docs/?dv=osx

---

### install extensions

click on extension within VSC (visual studio code)

- install python
- install Django Templates and backend snipets
- install Django Template language support
- install Prettier code formatter
- install kite autocomplete
- install HTML Boilerplate
- install Bracket Pair Colorizer
- install Auto Rename Tag
- install CSS Peek
- install HTML CSS Support
- install Live Sass Compiler
- install Live Server
- install Visual Studio Live Share
- install Material Theme

---

### install kite copilot

read about kite
https://kite.com/

download and install kite copilot and run it
https://kite.com/download/

### set vscode settings.json for user

edit the settings file located below:
code ~/Library/Application\ Support/Code/User/settings.json

```
{
  "python.pythonPath": "${workspaceFolder}/.venv/bin/python",
  "python.linting.pylintPath": "${workspaceFolder}/.venv/bin/pylint",
  "python.linting.flake8Path": "${workspaceFolder}/.venv/bin/flake8",
  "python.formatting.blackPath": "${workspaceFolder}/.venv/bin/black",
  "kite.showWelcomeNotificationOnStartup": false,
  "terminal.integrated.fontSize": 13,
  "editor.fontSize": 13,
  "editor.tabSize": 2,
  "window.zoomLevel": 1,
  "terminal.integrated.cursorBlinking": true,
  "python.linting.enabled": true,
  "python.linting.flake8Enabled": true,
  "python.formatting.provider": "black",
  "editor.formatOnSave": true,
  "editor.formatOnPaste": true,
  "workbench.colorTheme": "Material Theme High Contrast",
  "explorer.confirmDragAndDrop": false,
  "[python]": {
    "editor.codeActionsOnSave": {
      "source.organizeImports": true
    }
  },

  "liveSassCompile.settings.formats": [
    {
      "format": "expanded",
      "extensionName": ".css",
      "savePath": "~/../css/"
    }
  ]
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

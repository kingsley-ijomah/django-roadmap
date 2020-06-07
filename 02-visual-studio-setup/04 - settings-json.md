### set vscode settings.json for user

### read about settings here:

https://code.visualstudio.com/docs/getstarted/settings
https://code.visualstudio.com/docs/python/linting#_enable-linters

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

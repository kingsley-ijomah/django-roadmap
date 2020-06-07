## install python

### install brew and pyenv

https://brew.sh/

brew update
brew install pyenv

### install pyenv

pyenv install 3.8.2

### check what shell you are using

`echo $0`

### put this in .zshrc (zsh) / .bash_profile (bash) / .bashrc (ubuntu desktop)

<!-- put pyenv path into shell -->
<!-- put in shell to enable shims and autocompletion -->

```
echo -e 'export PATH="$HOME/.pyenv/bin:$PATH"' >> ~/.zshrc`

echo -e 'if command -v pyenv 1>/dev/null 2>&1; then\n eval "$(pyenv init -)"\nfi' >> ~/.zshrc
```

### refresh shell

`exec "$SHELL"`

### check versions and set global

pyenv ( list of commands )
pyenv versions
pyenv global 3.8.2
python --version

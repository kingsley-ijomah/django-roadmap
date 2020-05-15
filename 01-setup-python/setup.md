### install python

## get latest python
http://stackoverflow.com/questions/18671253/how-can-i-use-homebrew-to-install-both-python-2-and-3-on-mac

brew install pyenv
pyenv install 3.8.1

## put this in .zshrc
export PATH="$HOME/.pyenv/bin:$PATH"
eval "$(pyenv init -)"
eval "$(pyenv virtualenv-init -)"


## check versions and set global
pyenv versions

## set global
pyenv global 3.8.1
python --version

## install env
pip install env

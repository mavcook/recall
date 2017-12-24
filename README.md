# Recall
Command line tool for helping you remember the things you always forget.
[On pypi](https://pypi.python.org/pypi/recall-cmds)

## Install
```
pip install recall-cmds
```
## Use
```
$ recall
```

### Motivation
After setting up a 'forgets' file, inspired by [always_forget.txt](https://github.com/awdeorio/dotfiles/blob/master/.always_forget.txt), I found myself still forgetting the command I wanted when I exited the file. So I wanted a tool where I could view my .forgets file, easily select my forgotten command, so I could edit and execute it.

### Examples

# Features
## Assisted Editing
*In development*
Easily edit templated commands
```
recall -a
```
Will launch 
Any line that includes labels in double-curly-braces will auto prompt you to easily fill out your command
```
tar -zcvf{{additionalFlags}} {{finalName}}.tar.gz {{totar}}
additionalFlags:
finalName:
toTar:
```
### Bash Autocomplete

## Navigation
### Search
### Goto

## Interface
### Better rendering (more pretty pls)

# Users
# Setup

# Built with / design

# Developing
## Setup
## Running tests
## Contributing

# Packaging
You need to have a ~/.pypirc file:
```
[distutils]
index-servers=
    testpypi
    pypi

[testpypi]
repository: https://test.pypi.org/legacy/
username: uname
password: pass

[pypi]
repository: https://upload.pypi.org/legacy/
username: uname2
password: pass2
```
## Testing
```
python setup.py sdist
twine upload dist/* -r testpypi
mkdir test && cd test && virtualenv -p python3 venv && source venv/bin/activate
pip install --index-url https://test.pypi.org/simple/ recall-cmds --no-cache-dir
```

## Upload
```
python setup.py sdist
twine upload dist/*
```

# Versioning
standalone executable
pip

# Support
If you like Recall and wish to support futher development, or support feeding my stomach, you can make a donation using the links below:

[Venmo @maverick-cook](https://venmo.com/Maverick-Cook?txn=pay&note=Supporting%20Recall)
[PayPal](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=9G7XP36AHAQ7Q&lc=US&item_name=Maverick%20Cook%20Developer%20Fund&item_number=mcdf2017&currency_code=USD&bn=PP%2dDonationsBF%3abtn_donate_SM%2egif%3aNonHosted)
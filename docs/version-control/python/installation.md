
# Installation Guideline

Install python version manager & package manager
Recommended choices are:

- Pyenv-win or Anaconda for Windows 
- Pyenv for Ubuntu & MacOS

Use the python version of your choice (global scope with your pvm)
Install virtualenv with pip (help you create a virtual environment)
Install pipenv with pip (package manager, helps you create and install packages to and from pipfile)

Go to the root folder of the project & create a virtual environment for your project

```bash
virtualenv .venv
```

From here you could use pipenv to add new packages to the pipfile and then use pipenv to install it.
Pipenv will automatically select the virtual environment you just created

- To install packages from pipfile

```bash
pipenv install --skip-lock # install from the pipfile
```

- To install packages from the lock file
```bash
pipenv install --ignore-pipfile
```

- To install all packages including dev-packages from the pipfile
```bash
pipenv install --dev
```

- To add new packages
```bash
pipenv install package-name
```

- To add new dev packages
```bash
pipenv install package-name --dev
```

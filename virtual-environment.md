# Python Environment

## Changing python environment

### Which python are you using?

After going into `python`, type

```python
import sys
sys.version
sys.executable
```

to see the directory of python it is running.

## Virtual environment

To install packages specific to a project, we use virtual environment. We don't want to change the global package so that it works for one project and breaks for another.

### Create a virtual environment (shell and `pip` commands)

- `python -m venv [env_name]` - creates virtual environment directory in current directory
- `[env_name]\Scripts\activate.bat` - activates the virtual environment
- `where python` to check which python is it using
- `pip list` - list all packages in the environment
- `pip list --local` - lists all packages in the local environment
- `pip install [package_name]` - installs package
- `pip freeze` - prints the package requirements in the environment
- `pip freeze > requirements.txt` - writes package requirements in the environment into `requirement.txt`
- `pip install -r requirements.txt` - (`-r` expects a requirement file) installs every required package listed
- `deactivate` - goes out of the virtual environment
- `rmdir [env_name] /s` - delete all stuff in virtual environment

It's common to put virtual environment inside project folder, but never put any project files in the virtual environment. The environment should not be committed and should be ignored.

### Virtual environment in Jupyter Notebook

#### Add venv

- `pip install --user ipykernel` - Install Jupyter Notebook kernel
- `python -m ipykernel install --user --name=myenv` - Add venv to Jupyter Notebook

#### Remove venv

- `jupyter kernelspec uninstall myenv` - Remove venv from Jupyter Notebook
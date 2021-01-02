# Configuring path variable (Windows)
To run python in command prompt, python needs to be added to the system's path variable. In Windows, go to:
- `setting > system > about > system information` or
- `control pannel > system and security > system`.

Then, go to `advanced system settings > environment variables`. In the user variables, click on `path`, then click `edit`. Add python directory in `path` and move up priority. (Do not type `python.exe`, directory only.) Be sure to save any changes.

Now, python is available by typing `python` in the command prompt, just like in anaconda prompt. To use python in `git bash`, type `python -i`.

To use `pip` in command prompt, follow the same steps described above. (The directory of `pip` is usually located in `Scripts` folder where `python.exe` is located.)

# Changing python environment
## Which python are you using?
After going into `python`, type
```python
import sys
sys.version
sys.executable
```
to see the directory of python it is running.

# Virtual environment
To install packages specific to a project, we use virtual environment. We don't want to change the global package so that it works for one project and breaks for another.

## Create a virtual environment (shell and `pip` commands)
- `python -m venv [env_name]` - creates virtual environment directory in current directory
- `[env_name]\Scripts\activate.bat` - activates the virtual environment
- `where python` to check which python is it using
- `pip list` - list all packages in the environment
- `pip list --local` - lists all packages in the local environment
- `pip install [package_name]` - installs package
- `pip freeze` - gives the package requirements in the environment (that can go into requirement.txt)
- `pip install -r requirements.txt` - (`-r` expects a requirement file) installs every required package listed
- `deactivate` - goes out of the virtual environment
- `rmdir [env_name] /s` - delete all stuff in virtual environment

It's common to put virtual environment inside project folder, but never put any project files in the virtual environment. The environment should not be committed and should be ignored.
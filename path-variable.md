# Configuring path variable (Windows)

To run python in command prompt, python needs to be added to the system's path variable. In Windows, go to:

- `setting > system > about > system information` or
- `control pannel > system and security > system`.

Then, go to `advanced system settings > environment variables`. In the user variables, click on `path`, then click `edit`. Add python directory in `path` and move up priority. (Do not type `python.exe`, directory only.) Be sure to save any changes.

Now, python is available by typing `python` in the command prompt, just like in anaconda prompt. To use python in `git bash`, type `python -i`.

To use `pip` in command prompt, follow the same steps described above. (The directory of `pip` is usually located in `Scripts` folder where `python.exe` is located.)

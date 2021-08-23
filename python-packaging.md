# Python Packaging

## Directory structure

The directory of the package should at least have:

- package directory
  - package-name
    - `__init__.py`
    - `some_module.py`
    - ...
  - `setup.py`
  - ...

## Packaging commands

When packaging, cd into the package directory and type

```bash
python setup.py bdist_wheel
```

to generate the distribution `.whl` wheel files. To upload the distribution to [PyPI](https://pypi.org/), type

```bash
python -m twine upload dist/*
```

which will prompt username and password for the PyPI account for uploading.

## Package local update

To upgrade the local package, use

```bash
pip install --upgrade PACKAGE_NAME
```

## Python package dependencies

To obtain detailed (direct and indirect) package dependencies of the package in a virtual environment for generating `requirements.txt`, type

```bash
pip list --format=freeze > requirements.txt
```

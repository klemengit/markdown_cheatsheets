# Create wheel for package installation

Upgrade `setuptools` and `wheel` package:
```
python -m pip install --user --upgrade setuptools wheel
```

Run in the same file where `setup.py` is located:
```
python setup.py sdist bdist_wheel
```

Go to `dist` file and run:
```
pip install <wheel_name>
```
to install the package.

# Uploading the package
The packaging process is described here: https://packaging.python.org/tutorials/packaging-projects/

To upload the files to PyPI first install Twine:
```
python -m pip install --user --upgrade twine
```
To upload the project to **test PyPI**, run:
```
python -m twine upload --repository-url https://test.pypi.org/legacy/ dist/*
```
To upload the project to **PyPI**, run:
```
python -m twine upload dist/*
```

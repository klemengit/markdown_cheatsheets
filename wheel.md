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



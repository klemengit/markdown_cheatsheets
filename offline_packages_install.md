If you want to install a bunch of dependencies from, say a requirements.txt, you would do:

You must have the `requirements.txt` file in the directory. Then in that directory do:
```
mkdir dependencies
pip download -r requirements.txt -d "./dependencies"
```

And, once you transfer the `dependencies` folder and `requirements.txt` to the machine which does not have internet you would do:
```
pip install --no-index --find-links ./dependencies -r ../requirements.txt
```
NOTE: *Maybe the `requirements.txt` is not necessary on the other machine.*

All of this can be don in a **virtual environment** for better package seperation.

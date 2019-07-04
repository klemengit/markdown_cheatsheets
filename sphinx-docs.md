# Make the auto docs with sphinx

https://medium.com/@richdayandnight/a-simple-tutorial-on-how-to-document-your-python-project-using-sphinx-and-rinohtype-177c22a15b5b

Follow the instructions. **Select yes for Makefile and windows file (make.bat)**

To make docs:
```
make html
```
to clear docs:
```
make clean
```

# Publish the docs to GitHub

Use `publish-sphinx-docs`

```
publish-sphinx-docs --docs-dir <path-to-source> --docs-remote <link-to-repo>
```

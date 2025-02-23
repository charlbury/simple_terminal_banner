# Contributing

## Processs

Clean previous builds: Remove any previous build artifacts to ensure a clean build

```
rm -rf dist build simple_terminal_banner.egg-info
```

Build the package: Use setuptools and wheel to build the package.

```
python setup.py sdist bdist_wheel
```

Upload to PyPI: Once you have tested the package on Test PyPI, you can upload it to the official PyPI repository.

```
python -m twine upload dist/*
```

Tag the release: Create a tag for the new version of your package in VS Code git graph.

Create a release on GitHub: Go to your GitHub repository and create a new release using the tag you just created. Include detailed release notes that describe the changes, new features, bug fixes, and any other relevant information for this version

Perhaps use the format below:

```
# Release v0.1.0

## Changes
- Added new themes: `HASH`, `STAR`, `SPACE`, `NONE`
- Improved banner display logic
- Fixed issue with title truncation
- Added more unit tests

## Installation
You can install the latest version using pip:
```sh
pip install simple_terminal_banner
```
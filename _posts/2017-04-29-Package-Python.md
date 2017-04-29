---
title: "Packages In Python"
---

Implementing packages in python

### Creating packages in Python
- Create a directory with should be under sys.path
- Create a __init__.py file for the packages
- import packages
- type(package)
- Package is just a directory
- Create a new file (Reader.py) in reader packages
- Create a Reader class in Reader.py

### Adding a subpackage in Reader package
- Add a sub directory in reader folder
- `import reader`
- `import reader.compressed`
- `import reader.compressed.gzipped`

### Package Review
1. Packages are modules that contain other modules.
2. Packages are implemented as directories containing __init__.py file.
3. __init__.py file is executed when the package is imported.
4. Packages can contain sub packages.

### Difference between absolute import and relative import
- **absolute imports**
  - impots which use a full path to the module
  - from reader.reader import reader
- **relative imports**
  - imports which use a relative path to modules in the same package.
  - from .reader import Reader
  - each dot stands for a package in higher directory (similar to directory structure)
  - from . import common

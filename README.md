# papermc-updater

A command-line tool to update a PaperMC server .jar file (in-place) to the latest build. Supports latest and previous MC versions.

## Installation

Requires Python 3.10+.

### From PyPI

```
$ python -m pip install papermc-updater
```

or

```
$ pip install papermc-updater
```

### From source

```
$ git clone https://github.com/tjkessler/papermc-updater
$ cd papermc-updater
$ python -m pip install .
```

## Usage

Warning: this tool replaces the existing PaperMC server .jar file!

### Command line

```
$ update-papermc $PATH_TO_EXISTING_JARFILE
```

The default MC version is `1.20.1` - specify a different MC version with:

```
$ update-papermc $PATH_TO_EXISTING_JARFILE --version 1.19.4
```

### Python script

```python
from papermc_updater import update_paper_to_latest

update_paper_to_latest("$PATH_TO_EXISTING_JARFILE", version="1.20.1")
```

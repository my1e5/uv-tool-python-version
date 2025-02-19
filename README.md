# MRE

```
$ uv --version
uv 0.6.1 (c91ee82a8 2025-02-17)
```
```
$ uv init --app --package uv-tool-python-version --python 3.11
```
Change the `requires-python` field to
```
requires-python = "==3.11.*"
```
Install using `uv tool install`

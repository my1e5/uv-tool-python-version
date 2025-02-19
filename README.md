# Run

```
uv -v tool install git+https://github.com/my1e5/uv-tool-python-version
```
or `uvx git+...` or `uv tool run git+...`

## Logs

Note how it doesn't use Python 3.11 even though `requires-python` is set to `==3.11.*`.

```
❯ uv -v tool install git+https://github.com/my1e5/uv-tool-python-version
DEBUG uv 0.6.1 (c91ee82a8 2025-02-17)
DEBUG Searching for default Python interpreter in managed installations or search path
DEBUG Searching for managed installations at `/Users/rd/.local/share/uv/python`
DEBUG Found managed installation `cpython-3.13.1-macos-aarch64-none`
DEBUG Found `cpython-3.13.1-macos-aarch64-none` at `/Users/rd/.local/share/uv/python/cpython-3.13.1-macos-aarch64-none/bin/python3.13` (managed installations)
DEBUG Using request timeout of 30s
DEBUG Attempting GitHub fast path for: https://api.github.com/repos/my1e5/uv-tool-python-version/commits/HEAD
DEBUG Attempting to fetch `pyproject.toml` from: https://raw.githubusercontent.com/my1e5/uv-tool-python-version/bd950a7a0050587f64871ce3a44a4ba277817eb8/pyproject.toml
DEBUG Found static metadata via GitHub fast path for: git+https://github.com/my1e5/uv-tool-python-version
DEBUG Acquired lock for `/Users/rd/.local/share/uv/tools`
DEBUG Checking for Python environment at `/Users/rd/.local/share/uv/tools/uv-tool-python-version`
DEBUG Using request timeout of 30s
DEBUG Solving with installed Python version: 3.13.1
DEBUG Solving with target Python version: >=3.13.1
DEBUG Adding direct dependency: uv-tool-python-version*
DEBUG Searching for a compatible version of uv-tool-python-version @ git+https://github.com/my1e5/uv-tool-python-version (*)
DEBUG Tried 1 versions: uv-tool-python-version 1
DEBUG marker environment resolution took 0.002s
Resolved 1 package in 6ms
DEBUG Creating environment for tool `uv-tool-python-version`: /Users/rd/.local/share/uv/tools/uv-tool-python-version
DEBUG Assessing Python executable as base candidate: /Users/rd/.local/share/uv/python/cpython-3.13.1-macos-aarch64-none/bin/python3.13
DEBUG Using base executable for virtual environment: /Users/rd/.local/share/uv/python/cpython-3.13.1-macos-aarch64-none/bin/python3.13
DEBUG Using request timeout of 30s
DEBUG Identified uncached distribution: uv-tool-python-version @ git+https://github.com/my1e5/uv-tool-python-version@bd950a7a0050587f64871ce3a44a4ba277817eb8
DEBUG Fetching source distribution from Git: https://github.com/my1e5/uv-tool-python-version
DEBUG Acquired lock for `https://github.com/my1e5/uv-tool-python-version`
DEBUG Updating Git source `https://github.com/my1e5/uv-tool-python-version`
   Updating https://github.com/my1e5/uv-tool-python-version (HEAD)
DEBUG Skipping GitHub fast path; full commit hash provided: bd950a7a0050587f64871ce3a44a4ba277817eb8
DEBUG Performing a Git fetch for: https://github.com/my1e5/uv-tool-python-version
DEBUG Reset /Users/rd/.cache/uv/git-v0/checkouts/d8f1770f833e24d2/bd950a7 to bd950a7a0050587f64871ce3a44a4ba277817eb8
    Updated https://github.com/my1e5/uv-tool-python-version (bd950a7a0050587f64871ce3a44a4ba277817eb8)
DEBUG Released lock at `/Users/rd/.cache/uv/git-v0/locks/d8f1770f833e24d2`
DEBUG Acquired lock for `/Users/rd/.cache/uv/sdists-v8/git/6a3d0dfc4bfb1a27/bd950a7a0050587f`
   Building uv-tool-python-version @ git+https://github.com/my1e5/uv-tool-python-version@bd950a7a0050587f64871ce3a44a4ba277817eb8
DEBUG Building: uv-tool-python-version @ git+https://github.com/my1e5/uv-tool-python-version@bd950a7a0050587f64871ce3a44a4ba277817eb8
DEBUG No workspace root found, using project root
DEBUG Assessing Python executable as base candidate: /Users/rd/.local/share/uv/python/cpython-3.13.1-macos-aarch64-none/bin/python3.13
DEBUG Using base executable for virtual environment: /Users/rd/.local/share/uv/python/cpython-3.13.1-macos-aarch64-none/bin/python3.13
DEBUG Ignoring empty directory
DEBUG Resolving build requirements
DEBUG Solving with installed Python version: 3.13.1
DEBUG Solving with target Python version: >=3.13.1
DEBUG Adding direct dependency: hatchling*
DEBUG Found stale response for: https://pypi.org/simple/hatchling/
DEBUG Sending revalidation request for: https://pypi.org/simple/hatchling/
DEBUG Found not-modified response for: https://pypi.org/simple/hatchling/
DEBUG Searching for a compatible version of hatchling (*)
DEBUG Selecting: hatchling==1.27.0 [compatible] (hatchling-1.27.0-py3-none-any.whl)
DEBUG Found fresh response for: https://files.pythonhosted.org/packages/08/e7/ae38d7a6dfba0533684e0b2136817d667588ae3ec984c1a4e5df5eb88482/hatchling-1.27.0-py3-none-any.whl.metadata
DEBUG Adding transitive dependency for hatchling==1.27.0: packaging>=24.2
DEBUG Adding transitive dependency for hatchling==1.27.0: pathspec>=0.10.1
DEBUG Adding transitive dependency for hatchling==1.27.0: pluggy>=1.0.0
DEBUG Adding transitive dependency for hatchling==1.27.0: trove-classifiers*
DEBUG Found stale response for: https://pypi.org/simple/packaging/
DEBUG Sending revalidation request for: https://pypi.org/simple/packaging/
DEBUG Found stale response for: https://pypi.org/simple/pathspec/
DEBUG Sending revalidation request for: https://pypi.org/simple/pathspec/
DEBUG Found stale response for: https://pypi.org/simple/pluggy/
DEBUG Sending revalidation request for: https://pypi.org/simple/pluggy/
DEBUG Found stale response for: https://pypi.org/simple/trove-classifiers/
DEBUG Sending revalidation request for: https://pypi.org/simple/trove-classifiers/
DEBUG Found not-modified response for: https://pypi.org/simple/pluggy/
DEBUG Found not-modified response for: https://pypi.org/simple/trove-classifiers/
DEBUG Found not-modified response for: https://pypi.org/simple/pathspec/
DEBUG Found not-modified response for: https://pypi.org/simple/packaging/
DEBUG Found fresh response for: https://files.pythonhosted.org/packages/88/5f/e351af9a41f866ac3f1fac4ca0613908d9a41741cfcf2228f4ad853b697d/pluggy-1.5.0-py3-none-any.whl.metadata
DEBUG Found fresh response for: https://files.pythonhosted.org/packages/e1/67/038a8c7f60ffd6037374649826dbaa221e4b17755016b71a581162a15ce1/trove_classifiers-2025.2.18.16-py3-none-any.whl.metadata
DEBUG Searching for a compatible version of packaging (>=24.2)
DEBUG Selecting: packaging==24.2 [compatible] (packaging-24.2-py3-none-any.whl)
DEBUG Found fresh response for: https://files.pythonhosted.org/packages/cc/20/ff623b09d963f88bfde16306a54e12ee5ea43e9b597108672ff3a408aad6/pathspec-0.12.1-py3-none-any.whl.metadata
DEBUG Found fresh response for: https://files.pythonhosted.org/packages/88/ef/eb23f262cca3c0c4eb7ab1933c3b1f03d021f2c48f54763065b6f0e321be/packaging-24.2-py3-none-any.whl.metadata
DEBUG Searching for a compatible version of pathspec (>=0.10.1)
DEBUG Selecting: pathspec==0.12.1 [compatible] (pathspec-0.12.1-py3-none-any.whl)
DEBUG Searching for a compatible version of pluggy (>=1.0.0)
DEBUG Selecting: pluggy==1.5.0 [compatible] (pluggy-1.5.0-py3-none-any.whl)
DEBUG Searching for a compatible version of trove-classifiers (*)
DEBUG Selecting: trove-classifiers==2025.2.18.16 [compatible] (trove_classifiers-2025.2.18.16-py3-none-any.whl)
DEBUG Tried 5 versions: hatchling 1, packaging 1, pathspec 1, pluggy 1, trove-classifiers 1
DEBUG marker environment resolution took 0.087s
DEBUG Installing in pluggy==1.5.0, pathspec==0.12.1, trove-classifiers==2025.2.18.16, packaging==24.2, hatchling==1.27.0 in /Users/rd/.cache/uv/builds-v0/.tmpiamIIh
DEBUG Registry requirement already cached: pluggy==1.5.0
DEBUG Registry requirement already cached: pathspec==0.12.1
DEBUG Registry requirement already cached: trove-classifiers==2025.2.18.16
DEBUG Registry requirement already cached: packaging==24.2
DEBUG Registry requirement already cached: hatchling==1.27.0
DEBUG Installing build requirements: pluggy==1.5.0, pathspec==0.12.1, trove-classifiers==2025.2.18.16, packaging==24.2, hatchling==1.27.0
DEBUG Creating PEP 517 build environment
DEBUG Calling `hatchling.build.get_requires_for_build_wheel()`
DEBUG No workspace root found, using project root
DEBUG Calling `hatchling.build.build_wheel("/Users/rd/.cache/uv/builds-v0/.tmpgVzI5W", {}, None)`
DEBUG Finished building: uv-tool-python-version @ git+https://github.com/my1e5/uv-tool-python-version@bd950a7a0050587f64871ce3a44a4ba277817eb8
      Built uv-tool-python-version @ git+https://github.com/my1e5/uv-tool-python-version@bd950a7a0050587f64871ce3a44a4ba277817eb8
DEBUG Released lock at `/Users/rd/.cache/uv/sdists-v8/git/6a3d0dfc4bfb1a27/bd950a7a0050587f/.lock`
Prepared 1 package in 1.64s
Installed 1 package in 2ms
 + uv-tool-python-version==0.1.0 (from git+https://github.com/my1e5/uv-tool-python-version@bd950a7a0050587f64871ce3a44a4ba277817eb8)
DEBUG Installing tool executables into: /Users/rd/.local/bin
DEBUG Looking at `.dist-info` at: /Users/rd/.local/share/uv/tools/uv-tool-python-version/lib/python3.13/site-packages/uv_tool_python_version-0.1.0.dist-info
DEBUG Installing executable: `uv-tool-python-version`
Installed 1 executable: uv-tool-python-version
DEBUG Adding receipt for tool `uv-tool-python-version`
DEBUG Adding metadata entry for tool `uv-tool-python-version` at /Users/rd/.local/share/uv/tools/uv-tool-python-version/uv-receipt.toml
DEBUG Released lock at `/Users/rd/.local/share/uv/tools/.lock`
```


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

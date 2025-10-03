# 2025-python

https://github.com/kaunjovi/2025-python


## uv 
1. https://realpython.com/uv-vs-pip/
1. https://pypi.org/project/uv/

1. Implementation Rust

1. Update the version of uv 
```
uv self update
info: Checking for updates...
success: Upgraded uv from v0.7.13 to v0.8.22! https://github.com/astral-sh/uv/releases/tag/0.8.22
```

1. Check the version of uv 

```
uv self version
uv 0.8.22 (ade2bdbd2 2025-09-23)
```

1. Initialize a project with uv 

```
uv init 2025-python/
Initialized project `2025-python` at `/Users/kaunjovi/code/2025-python/`
```

1. Which all version of Python is installed in the machine. 

```
uv python list --only-installed
cpython-3.12.11-macos-aarch64-none    /opt/homebrew/bin/python3.12 -> ../Cellar/python@3.12/3.12.11/bin/python3.12
cpython-3.11.9-macos-aarch64-none     /usr/local/bin/python3.11 -> ../../../Library/Frameworks/Python.framework/Versions/3.11/bin/python3.11
cpython-3.11.9-macos-aarch64-none     /usr/local/bin/python3 -> ../../../Library/Frameworks/Python.framework/Versions/3.11/bin/python3
cpython-3.11.9-macos-aarch64-none     /Library/Frameworks/Python.framework/Versions/3.11/bin/python3.11
cpython-3.11.9-macos-aarch64-none     /Library/Frameworks/Python.framework/Versions/3.11/bin/python3 -> python3.11
cpython-3.9.6-macos-aarch64-none      /usr/bin/python3
```

1. I like to go with 3.12 and not 3.11, the current one. Also 3.13 seems dicey. 

```
uv python pin 3.12

Updated `.python-version` from `3.11` -> `3.12`
```

1. Now I want to make a new venv. Ok, **manually** delete the old one. Leave the python-version. Create a new venv and activate it.  

```
uv venv
Using CPython 3.12.11 interpreter at: /opt/homebrew/opt/python@3.12/bin/python3.12
Creating virtual environment at: .venv
Activate with: source .venv/bin/activate
```

1. run  

```
uv run main.py
Hello from 2025-python!
```



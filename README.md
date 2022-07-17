# public-python-packages #

Centralised hosting for public python packages (eg. that aren't hosted on pypi)

## Brainstem #

There is no public package on pypi: https://pypi.org/project/brainstem/

Instead, you have to [download their SDK](https://acroname.com/software/brainstem-development-kit) and extract the `.whl` files (now hosted here)

### Usage ###

To use the Brainstem library in your project, add the following to your Pipfile `[packages]` section:

```
brainstem = {file = "https://github.com/UBCO-Bikes/public-python-packages/raw/master/brainstem/linux/brainstem-2.9.3-py2.py3-none-any.whl", sys_platform = "== 'linux'"}
brainstem_win = {file = "https://github.com/UBCO-Bikes/public-python-packages/raw/master/brainstem/win/brainstem-2.9.4-py2.py3-none-any.whl", sys_platform = "== 'win32'"}
```

This ensures the correct package is used for your platform.

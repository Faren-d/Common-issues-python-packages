# Common-issues-python-packages

Use ```-m``` when:

- You get package/import errors
- You're running a file that's part of a package
- You need relative imports to work

  ## i.e.

```python my_project/main.py```

```python -m my_project.main```

## Simple Rule:

Without ```-m```: Python runs the file directly.

With ```-m```: Python runs the file as part of a package.

## Quick checklist - Use ```-m``` when:

✅ You see "No module named..." errors

✅ You're using relative imports (with dots)

✅ Your file is part of a larger package

✅ You need ```__package__``` to be set correctly

## Don't need ```-m``` when:

❌ Running standalone scripts

❌ Using only absolute imports

❌ Running files not part of a package

### ```os.getcwd()```
```bash
import os
print(os.getcwd())
```
## what it shows?
- Shows your Current Working Directory (CWD)
- It's like asking "Where am I right now?"
- Returns a single path as a string
- Useful when you need to know where Python is running from

### ```sys.path```
 ```bash
import sys
print(sys.path)
```
## what it shows?
- Shows all directories where Python looks for modules to import
- It's like your Python "search path"
- Returns a list of multiple paths
- The first entry (sys.path[0]) is usually the same as os.getcwd()

- os.getcwd() is like your current address
- sys.path is like a list of all places you're allowed to get things from

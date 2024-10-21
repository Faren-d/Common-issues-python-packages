# Common-issues-python-packages
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

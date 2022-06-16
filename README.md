<h1 align="center">
	<img src="https://cdn-icons-png.flaticon.com/512/892/892794.png" width="150px"><br>
    Mation - An object-oriented binary to decimal utility.
</h1>
<p align="center">
    Mation allows you to easily add binary and convert it to decimal.
</p>

<h1></h1>

**Install**

```
git clone https://github.com/ftr4ce/Mation.git
```

<h1></h1>

**Code Example**

```python
import sys
from Mation import Mation

# With sys arguments

if len(sys.argv) < 3:
		exit(f"Error: No arguments found\nUsage: {sys.argv[0]} number1 number2")

M = Mation()
D = M.binAdd(sys.argv[1], sys.argv[2])
M.prettyPrint(sys.argv[1], sys.argv[2], D)
```
```python
from Mation import Mation

# With inputs

first = input("Enter the first number: ")
second = input("Enter the second number: ")

try:
    M = Mation()
    D = M.binAdd(first, second)
    M.prettyPrint(first, second, D)
except ValueError:
    exit(f"\nError: No arguments found\nUsage: filename.py number1 number2")
```

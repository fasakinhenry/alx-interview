# 0x00. Pascal's Triangle

`Algorithm` `Python` `Encapsulation`

## General Requirements

- Allowed editors: `vi`, `vim`, `emacs`
- Files would be interpreted/compiled on Ubuntu 14.04 LTS using `python3` (version 3.4.3)
- First line of each python file should be shebang `#!/usr/bin/python3`
- `README.md` file at root of repository and in every directory is mandatory
- Code should be documented and should use `PEP 8` style (version 1.7.x)
- Files must be executable

## Tasks

### 0. Pascal's Triangle

`mandatory`

Create a function def pascal_triangle(n): that returns a list of lists of integers representing the Pascal’s triangle of n:

- Returns an empty list if n <= 0
- You can assume n will be always an integer

```bash
guillaume@ubuntu:~/0x00$ cat 0-main.py
#!/usr/bin/python3
"""
0-main
"""
pascal_triangle = __import__('0-pascal_triangle').pascal_triangle

def print_triangle(triangle):
    """
    Print the triangle
    """
    for row in triangle:
        print("[{}]".format(",".join([str(x) for x in row])))


if __name__ == "__main__":
    print_triangle(pascal_triangle(5))

guillaume@ubuntu:~/0x00$ 
guillaume@ubuntu:~/0x00$ ./0-main.py
[1]
[1,1]
[1,2,1]
[1,3,3,1]
[1,4,6,4,1]
guillaume@ubuntu:~/0x00$ 
```

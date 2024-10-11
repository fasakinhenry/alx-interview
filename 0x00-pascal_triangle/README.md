# 0x00. Pascal's Triangle

`Algorithm` `Python` `Encapsulation`

Pascal's Triangle is a triangular array of numbers where each number is the sum of the two numbers directly above it. The triangle starts with a single 1 at the top, and each subsequent row contains one more element than the previous row.

Here is a step-by-step description of how Pascal's Triangle is constructed:

1. **First Row**: The first row contains a single element, which is 1.
2. **Subsequent Rows**: Each subsequent row starts and ends with 1. Each interior element is the sum of the two elements directly above it from the previous row.

For example, the first few rows of Pascal's Triangle look like this:

```
    1
   1 1
  1 2 1
 1 3 3 1
1 4 6 4 1
```
Properties of Pascal's Triangle:

- **Symmetry**: Each row is symmetric.
- **Binomial Coefficients**: The elements of the nth row correspond to the coefficients of the binomial expansion ((a + b)^n).
- **Sum of Rows**: The sum of the elements in the nth row is (2^n).

Problem Statement:
Create a function def pascal_triangle(n): that returns a list of lists of integers representing the Pascal’s triangle of n:

If n <= 0, return an empty list.
Assume n is always an integer.
Example:
For n = 5, the function should return:
```
[
 [1],
 [1, 1],
 [1, 2, 1],
 [1, 3, 3, 1],
 [1, 4, 6, 4, 1]
]
```

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

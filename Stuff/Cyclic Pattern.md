where any four bytes at any point in the pattern are unique

[[wget]] https://raw.githubusercontent.com/Svenito/exploit-pattern/master/pattern.py
This is a cyclic pattern tool

Useful for determining the special characters in a [[Buffer Overflow]]

```
$ python3 pattern.py 0x41326441
```
This command tells u at what position the ascii representation of the hex shows up 
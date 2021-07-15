Chapter B
==========
（察するPython入門）

B01
---

### B010
```py
print(2 > 1)
print(2 < 1)
print(2 >= 1)
print(2 <= 1)
print(2 == 1)
print(2 != 1)
```
```txt
True
False
True
False
False
True
```

### B011
```py
print(type(2 > 1))
```
```txt
<class 'bool'>
```

### B012
```py
print(2 = 1)
```
(error)
```txt
    print(2 = 1)
          ^
SyntaxError: expression cannot contain assignment, perhaps you meant "=="?
```

### B013
```py
x = 2
print(1 < x < 3)
```
```txt
True
```

### B014
```py
x = 4
print(1 < x and x < 3)
print(1 < x or x < 3)
print(not 1 < x)
```
```txt
False
True
False
```

### B015
```py
x = 4
print(not 1 < x)
print(not 1 < x and x < 3)
print(not (1 < x and x < 3))
print(x < 5 or 1 < x and x < 3)
```
```txt
False
False
True
True
```

B02
---

### B020
```py
if True:
    print("hello!")

print("bye!")
```
```txt
hello!
bye!
```

### B021
```py
if False:
    print("hello!")

print("bye!")
```
```txt
bye!
```
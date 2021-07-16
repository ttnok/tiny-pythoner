Chapter C
==========
（察するPython入門）

C01
---

### C010
Ctrl + C to stop
```py
while True:
    x = float(input("x: "))

    if x > 0:
        print(f"{x} > 0")
    else:
        print(f"{x} <= 0")
```
<pre>
<code>
x: <em>5↩️</em>
5.0 > 0
x: <em>-2↩️</em>
-2.0 <= 0
x: <em>3↩️</em>
3.0 > 0
...
x: <em>[Ctrl + C]</em>
</code>
</pre>

### C011
Enter 'q' to quit.
```py
x = input("x: ")

while x != "q":
    x = float(x)

    if x > 0:
        print(f"{x} > 0")
    else:
        print(f"{x} <= 0")

    x = input("x: ")

print("bye!")
```
<pre>
<code>
x: <em>5↩️</em>
5.0 > 0
x: <em>-2↩️</em>
-2.0 <= 0
x: <em>q↩️</em>
bye!
</code>
</pre>

### C012
Enter 'q' to quit.
```py
while True:
    x = input("x: ")

    if x == "q":
        break

    x = float(x)

    if x > 0:
        print(f"{x} > 0")
    else:
        print(f"{x} <= 0")

print("bye!")
```
<pre>
<code>
x: <em>5↩️</em>
5.0 > 0
x: <em>-2↩️</em>
-2.0 <= 0
x: <em>q↩️</em>
bye!
</code>
</pre>

### C013
```py
for _ in range(3):
    x = float(input("x: "))

    if x > 0:
        print(f"{x} > 0")
    else:
        print(f"{x} <= 0")

print("bye!")
```
<pre>
<code>
x: <em>5↩️</em>
5.0 > 0
x: <em>-2↩️</em>
-2.0 <= 0
x: <em>3↩️</em>
3.0 > 0
x: <em>q↩️</em>
bye!
</code>
</pre>

C02
---
### C020
```py
for i in range(3):
    print(i)

print("bye!")
```
```txt
0
1
2
bye!
```

### C021
```py
for i in range(1, 10, 1):
    print(i)

print("bye!")
```
```txt
1
2
3
4
5
6
7
8
9
bye!
```

### C022
```py
for i in range(1, 10, 2):
    print(i)

print("bye!")
```
```txt
1
3
5
7
9
bye!
```

### C023
```py
for i in range(10):
    print(2 * i + 1)

print("bye!")
```
```txt
1
3
5
7
9
11
13
15
17
19
bye!
```

### C024
```py
for i in range(10):
    print(f"{i} * {i} = {i ** 2}")

print("bye!")
```
```txt
0 * 0 = 0
1 * 1 = 1
2 * 2 = 4
3 * 3 = 9
4 * 4 = 16
5 * 5 = 25
6 * 6 = 36
7 * 7 = 49
8 * 8 = 64
9 * 9 = 81
bye!
```

### C025
```py
for i in range(10):
    print(f"{i} * {i} = {i ** 2:2d}")

print("bye!")
```
```txt
0 * 0 =  0
1 * 1 =  1
2 * 2 =  4
3 * 3 =  9
4 * 4 = 16
5 * 5 = 25
6 * 6 = 36
7 * 7 = 49
8 * 8 = 64
9 * 9 = 81
bye!
```

C03
---

### C030

```py
for i in range(3):
    print("the outer loop")
    print(f"i = {i}")
    for j in range(3):
        print("    the inner loop")
        print(f"    j = {j}")

print("bye!")
```
```txt
the outer loop
i = 0
    the inner loop
    j = 0
    the inner loop
    j = 1
    the inner loop
    j = 2
the outer loop
i = 1
    the inner loop
    j = 0
    the inner loop
    j = 1
    the inner loop
    j = 2
the outer loop
i = 2
    the inner loop
    j = 0
    the inner loop
    j = 1
    the inner loop
    j = 2
bye!
```

### C031
```py
for i in range(1, 3+1):
    for j in range(1, 3+1):
        print(f"{i} * {j} = {i * j:2d}")

print("bye!")
```
```txt
1 * 1 =  1
1 * 2 =  2
1 * 3 =  3
2 * 1 =  2
2 * 2 =  4
2 * 3 =  6
3 * 1 =  3
3 * 2 =  6
3 * 3 =  9
bye!
```

### C032
```py
for i in range(1, 9+1):
    for j in range(1, 9+1):
        print(f"{i * j:2d} ", end="")

    print()

print("bye!")
```
```txt
 1  2  3  4  5  6  7  8  9 
 2  4  6  8 10 12 14 16 18 
 3  6  9 12 15 18 21 24 27 
 4  8 12 16 20 24 28 32 36 
 5 10 15 20 25 30 35 40 45 
 6 12 18 24 30 36 42 48 54 
 7 14 21 28 35 42 49 56 63 
 8 16 24 32 40 48 56 64 72 
 9 18 27 36 45 54 63 72 81 
bye!
```

C04
---

### C040
```py
factorial = 1
n = 4

for i in range(1, n + 1):
    factorial = factorial * i

print(factorial)
```
```txt
24
```

### C041
```py
factorial = 1
n = 4

for i in range(1, n + 1):
    factorial = factorial * i
    print(f"{i}! = {factorial}")

print("bye!")
```
```txt
1! = 1
2! = 2
3! = 6
4! = 24
bye!
```

### C042
```py
factorial = 1
n = 4

for i in range(1, n + 1):
    print("1", end="")
    for j in range(1 + 1, i + 1):
        print(f" * {j}", end="")
    
    factorial = factorial * i
    print(f" = {factorial}")

print("bye!")
```
```txt
1 = 1
1 * 2 = 2
1 * 2 * 3 = 6
1 * 2 * 3 * 4 = 24
bye!
```

### C043
```py
factorial = 1
n = 4
s = "1"

for i in range(1 + 1, n + 1):    
    factorial = factorial * i
    s = f"{s} * {i}"
    print(f"{s} = {factorial}")

print("bye!")
```
```txt
1 * 2 = 2
1 * 2 * 3 = 6
1 * 2 * 3 * 4 = 24
bye!
```
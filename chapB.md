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
    print(2 = 1)  # error
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

### B022
```py
if 1 < 2:
    print("hello!")

print("bye!")

if 1 > 2:
    print("hello!")

print("bye!")
```
```txt
hello!
bye!
bye!
```

### B023
```py
x = float(input("x: "))

if x > 0:
    print(f"{x} > 0")

print("bye!")
```
<pre>
<code>
x: <em>5↩️</em>
5.0 > 0
bye!
</code>
</pre>

<pre>
<code>
x: <em>-2↩️</em>
bye!
</code>
</pre>

### B024
```py
x = float(input("x: "))

if x > 0:
    print(f"{x} > 0")

print("bye!")

if x <= 0:
    print(f"{x} <= 0")

print("bye!")
```
<pre>
<code>
x: <em>5↩️</em>
5.0 > 0
bye!
bye!
</code>
</pre>

<pre>
<code>
x: <em>-2↩️</em>
bye!
-2 <= 0
bye!
</code>
</pre>

### B025
```py
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
</code>
</pre>

<pre>
<code>
x: <em>-2↩️</em>
-2 <= 0
</code>
</pre>

B03
---

### B030
```py
x = float(input("x: "))

if x > 2.0:
    print(f"[{x}] > 2.0")
elif x > 1.0:
    print(f"1.0 < [{x}] <= 2.0")
else:
    print(f"[{x}] <= 1.0")
```
<pre>
<code>
x: <em>3↩️</em>
[3.0] > 2.0
</code>
</pre>

<pre>
<code>
x: <em>1.5↩️</em>
1.0 < [1.5] <= 2.0
</code>
</pre>

<pre>
<code>
x: <em>0↩️</em>
[0.0] <= 1.0
</code>
</pre>

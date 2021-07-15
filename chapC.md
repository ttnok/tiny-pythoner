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

### C011
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

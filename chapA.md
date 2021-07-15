Chapter A
=========
（察するPython入門）

A01
---

### A010
```py
print("hello")
```
```txt
hello
```

### A011
```py
print('hello')
```
```txt
hello
```

### A012
```py
print("hello, " + "world!")
```
```txt
hello, world!
```

### A013
```py
print("1 + 1 = " + "2")
```
```txt
1 + 1 = 2
```

### A014
```py
print("1 + 1 = " + 2)
```
(error)
```txt
---------------------------------------------------------------------------
...
----> 1 print("1 + 1 = " + 2)

TypeError: can only concatenate str (not "int") to str
```

A02
---

### A020
```py
print(2 + 3)
```

```txt
5
```

### A021
```py
print(2 - 3)
```
```txt
-1
```

### A022
```py
print(2 * 3)
```
```txt
6
```

### A023
```py
print(2 / 3)
```
```txt
0.6666666666666666
```

### A024
```py
print(2 // 3)
```
```txt
0
```

### A025
```py
print(11 // 3)
```
```txt
3
```

### A026
```py
print(11 % 3)
```
```txt
2
```

### A027
```py
print(type(11 / 3))
```
```txt
float
```

### A028
```py
print(type(11 // 3)
```
```txt
int
```


A03
---

### A030
```py
print("1 + 1 = " + (1 + 1))
```
(error)
```txt
---------------------------------------------------------------------------
...
----> 1 print("1 + 1 = " + (1 + 1))

TypeError: can only concatenate str (not "int") to str
```

### A031
```py
print("1 + 1 = " + str(1 + 1))
```
```txt
1 + 1 = 2
```

### A032
```py
print(f"1 + 1 = {1 + 1}")
```
```txt
1 + 1 = 2
```


A04
---
### A040
```py
your_name = "Taro"

print("Hello, " + your_name + "-san!")
```
```txt
Hello, Taro-san!
```

### A041
```py
your_name = "Taro"

print(f"Hello, {your_name}-san!")
```
```txt
Hello, Taro-san!
```

### A042
```py
num1 = 2
num2 = 3

print(f"{num1} + {num2} = {num1 + num2}")
```
```txt
2 + 3 = 5
```

### A043
```py
print(num100)
```

(error)
```txt
---------------------------------------------------------------------------
...
----> 1 print(num100)

NameError: name 'num100' is not defined
```

### A044
```py
x = 1
y = 2 * x + 1

print(y)
```
```txt
3
```

### A045
```py
t = 2 * s + 1

s = 1
print(t)
```
(error)
```txt
---------------------------------------------------------------------------
...
----> 1 t = 2 * s + 1
      2 
      3 s = 1
      4 print(t)

NameError: name 's' is not defined
```

### A046
```py
x = 1
y = 2 * x + 1

print(y)

y = 3 * x + 5
```
```txt
3
```
A05
---

### A050
```py
your_name = input("your name: ")

print(f"Hello, {your_name}-san!")
```

<pre>
<code>
your name: <em>Taro↩️</em>
Hello, Taro-san!
</code>
</pre>

### A051
```py
num1 = input("num1: ")

print(num1 + 1)
```

(error)
<pre>
<code>
num1: <em>5↩️</em>
</code>
</pre>
```txt
---------------------------------------------------------------------------
...
      1 num1 = input("num1: ")
      2
----> 3 print(num1 + 1)

TypeError: can only concatenate str (not "int") to str
```
### A052
```py
num1 = int(input("num1: "))

print(num1 + 1)
```

<pre>
<code>
num1: <em>5↩️</em>
6
</code>
</pre>

### A053
```py
num1 = float(input("num1: "))

print(num1 + 1)
```

<pre>
<code>
num1: <em>5.3↩️</em>
6.3
</code>
</pre>

### A054
```py
num1 = input("num1: ")

print(type(num1))
```

<pre>
<code>
num1: <em>5↩️</em>
string
</code>
</pre>

### A055
```py
num1 = int(input("num1: "))
num2 = int(input("num2: "))

print(f"num1 + num2 = {num1} + {num2} = {num1 + num2}")
```

<pre>
<code>
num1: <em>2↩️</em>
num2: <em>3↩️</em>
num1 + num2 = 2 + 3 = 5
</code>
</pre>


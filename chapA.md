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
print('The sign says, "Hello, World!"')
```
```txt
The sign says, "Hello, World!"
```
### A013
```py
print("The sign says, "Hello, World!"")
```
(error)
```txt
print("The sign says, "Hello, World!"")
                       ^
SyntaxError: invalid syntax
```

### A014
```py
print("The sign says, \"Hello, World!\"")
```
```txt
The sign says, "Hello, World!"
```

### A015
```py
print("' ... single quotaion")
print("\" ... double quotaion")

print('\' ... single quotaion')
print('" ... double quotaion')
```
```txt
' ... single quotation
" ... double quotation
' ... single quotation
" ... double quotation
```

### A016
```py
print("hello, " + "world!")
```
```txt
hello, world!
```

### A017
```py
print("1 + 1 = " + "2")
```
```txt
1 + 1 = 2
```

### A018
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

### A019
```py
# あいさつをするプログラム
print("hello") # hello と表示
```
```txt
hello
```

A02
---

### A020
```py
print(11 + 3)
print(11 - 3)
print(11 * 3)
print(11 / 3)
```

```txt
14
8
33
3.6666666666666665
```

### A021
```py
print(11 // 3)
print(11 % 3)
```

```txt
3
2
```

### A022
```py
print(5 ** 2)
```

```txt
25
```

### A023
```py
print(1j * 1j)
```
```txt
(-1+0j)
```

### A024
```py
print(j * j)  # error
```
(error)
```txt
---------------------------------------------------------------------------
----> 1 print(j * j)

NameError: name 'j' is not defined
```

### A025
```py
print((1 + 1j) ** 2)
```
```txt
2j
```

### A026
```py
print(complex(1, 1) ** 2)
```
```txt
2j
```

A03
---

### A030
```py
print(type(3))
print(type(3.0))
```
```txt
<class 'int'>
<class 'float'>
```

### A031
```py
print(type(11 + 3))
print(type(11 - 3))
print(type(11 * 3))
print(type(11 / 3))
print(type(11 // 3))
print(type(11 % 3))
print(type(11 ** 3))
```
```txt
<class 'int'>
<class 'int'>
<class 'int'>
<class 'float'>
<class 'int'>
<class 'int'>
<class 'int'>
```

### A032
```py
print(type(11 + 3.0))
print(type(11 - 3.0))
print(type(11 * 3.0))
print(type(11 / 3.0))
print(type(11 // 3.0))
print(type(11 % 3.0))
print(type(11 ** 3.0))
```
```txt
<class 'float'>
<class 'float'>
<class 'float'>
<class 'float'>
<class 'float'>
<class 'float'>
<class 'float'>
```

### A033
```py
print(type(1j))
```
```txt
<class 'complex'>
```

### A034
```py
print(type("3"))
```
```txt
<class 'str'>
```

A04
---

### A040
```py
print("1 + 1 = " + (1 + 1)) # error
```
(error)
```txt
---------------------------------------------------------------------------
...
----> 1 print("1 + 1 = " + (1 + 1))

TypeError: can only concatenate str (not "int") to str
```

### A041
```py
print("1 + 1 = " + str(1 + 1))
```
```txt
1 + 1 = 2
```

### A042
```py
print(f"1 + 1 = {1 + 1}")
```
```txt
1 + 1 = 2
```


A05
---
### A050
```py
your_name = "Taro"

print("Hello, " + your_name + "-san!")
```
```txt
Hello, Taro-san!
```

### A051
```py
your_name = "Taro"

print(f"Hello, {your_name}-san!")
```
```txt
Hello, Taro-san!
```

### A052
```py
num1 = 2
num2 = 3

print(f"{num1} + {num2} = {num1 + num2}")
```
```txt
2 + 3 = 5
```

### A053
```py
print(num100) # error
```

(error)
```txt
---------------------------------------------------------------------------
...
----> 1 print(num100)

NameError: name 'num100' is not defined
```

### A054
```py
x = 1
y = 2 * x + 1

print(y)
```
```txt
3
```

### A055
```py
t = 2 * s + 1  # error

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

### A056
```py
x = 1
y = 2 * x + 1

print(y)

y = 3 * x + 5
```
```txt
3
```

### A057
```py
x = 1
x = 2 * x + 1

print(x)
```
```txt
3
```

A06
---

### A060
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

### A061
```py
num1 = input("num1: ")

print(num1 + 1)  # error
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
### A062
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

### A063
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

### A064
```py
num1 = input("num1: ")

print(type(num1))
```

<pre>
<code>
num1: <em>5↩️</em>
&lt;class 'str'&gt;
</code>
</pre>

### A065
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


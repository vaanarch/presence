## Python References

* Input
* Read files
* Write files

&nbsp;
&nbsp;
&nbsp;

I O refers to input and output. Print function, for example, is used to generate a standard output to the console. Below are some code samples dealing with input and output.

### Input
```python
name = input("What is your name?\n")
surname = input("what is your surname?\n")
print("Welcome {0} {1}!".format(name, surname))
```
```python
reply = input("Enter base and power, separated by spaces: ")
pieces = reply.split()
x = float(pieces[0])
y = float(pieces[1])
print("Power is equal {}".format(x**y))
```

&nbsp;

### Reading a file
```python
file = open("input.py")
for line in file:
    print(line)

file.close()

with open("input2.py) as f:
    for line in f:
        print(line)
```

&nbsp;

### Writing to a file
```python
with open("new.py", "w") as f:
    f.write('print("hello world")')

with open("new.py) as f:
    code = f.read()
    exec(code)

In Python, a function is a block of code that can be reused multiple times, and is used to perform a specific task. Functions are defined using the "def" keyword, followed by the function name and a set of parentheses, which may contain parameters. The code inside the function is indented, and the function is invoked (or called) by using its name followed by parentheses, possibly with some arguments inside.

Here is an example of a simple function that takes two numbers as parameters and returns their sum:

```python
def add(x, y):
    result = x + y
    return result

result = add(3, 4)
print(result) # 7
```

In the above example, "add" is the name of the function. The "x" and "y" are the parameters that are passed to the function when it is called. 
The code inside the function, "result = x + y", performs the task of adding the two numbers together. The return statement is used to return the result of the function.

Functions can also have default values for some or all of the parameters, which means that the caller can choose to provide a value or not. In this case, if the caller does not provide a value, the default value will be used instead. Here's an example of a function that has a default value for one of its parameters:

```python
def power(x, y=2):
    result = x ** y
    return result

result = power(3) # 3**2=9
print(result)
result = power(3,3) # 3**3=27
print(result)
```

In this example, "power" is the name of the function. The "x" is the parameter that is passed to the function when it is called, and "y" is the parameter with a default value of 2. 
The code inside the function, "result = x ** y", performs the task of raising the number x to the power of y.

Functions can also take an arbitrary number of arguments, which can be passed to the function in the form of a tuple, using the * operator, and keyword arguments, which can be passed to the function in the form of a dictionary, using the ** operator.
Here's an example of a function that takes an arbitrary number of arguments:

```python
def avg(*args):
    return sum(args)/len(args)

print(avg(1,2,3)) # 2.0
print(avg(1,2,3,4)) # 2.5
```

In this example, "avg" is the function name and *args is used to pass an arbitrary number of arguments which are passed to the function as a tuple. 
The code inside the function, "return sum(args)/len(args)" performs the task of returning the average of the passed arguments.

Functions are a powerful feature in Python, as they allow you to organize your code into smaller, reusable blocks and make it easier to understand and maintain.

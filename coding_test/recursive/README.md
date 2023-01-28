A recursive function is a function that calls itself, either directly or indirectly, in order to solve a problem. Recursive functions can be used to solve problems that can be broken down into smaller, similar subproblems.

Here is an example of a recursive function that calculates the factorial of a given number:

```python
def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n-1)

print(factorial(5)) # 120
```

In this example, the 'factorial' function is defined to take a single argument n, and it returns the factorial of n. 
The function uses a recursive approach to solve the problem of finding the factorial of a number. 
It checks whether the input number is 0, if yes it returns 1 as factorial of 0 is 1, 
otherwise it calls itself with an input of (n-1) and multiplies the result of that call with n.

Here is another example of a recursive function that calculates the Fibonacci sequence of a given number:

```python
def fibonacci(n):
    if n <= 1:
        return n
    else:
        return fibonacci(n-1) + fibonacci(n-2)

print(fibonacci(8)) # 21
```

In this example, the fibonacci function is defined to take a single argument n, and it returns the nth element of the Fibonacci sequence. 
The function uses a recursive approach to solve the problem of finding the Fibonacci sequence. 
It checks whether the input number is less than or equal to 1, if yes it returns n, 
otherwise it calls itself twice, once with an input of (n-1) and other with input of (n-2) and it adds the results of the two calls.

A recursive function must have a base case, which is a condition that stops the recursion, and a recursive case, 
which is a condition that calls the function again. If the base case is not defined, the function will call itself indefinitely 
and result in a stack overflow error.

Recursive functions are very powerful but can be computationally expensive as they may call the function many times with the same inputs, 
which is known as overlapping subproblems. To avoid this, you can use a technique called memoization, 
which stores the results of previous function calls and returns them instead of calling the function again.

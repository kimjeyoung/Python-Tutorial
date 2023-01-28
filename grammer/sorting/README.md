In Python, there are several ways to sort data, including the built-in sorted() function and the sort() method of lists.

The sorted() function returns a new sorted list from the items in an iterable. The original iterable is not modified. The basic syntax is:

```python
sorted(iterable, key=None, reverse=False)
```

* **iterable**: the data to be sorted, for example a list, tuple, or string
* **key**: a function that returns a value to use for sorting. For example, to sort a list of strings by their length, you could use the len function as the key.
* **reverse**: if True, the data will be sorted in descending order, otherwise it will be sorted in ascending order (default).

For example:

```python
# Sort a list of numbers in ascending order
numbers = [3, 1, 4, 2, 5]
sorted_numbers = sorted(numbers)
print(sorted_numbers) # [1, 2, 3, 4, 5]

# Sort a list of strings in descending order
words = ['apple', 'banana', 'cherry']
sorted_words = sorted(words, reverse=True)
print(sorted_words) # ['cherry', 'banana', 'apple']

# Sort a list of strings by length
words = ['apple', 'banana', 'cherry']
sorted_words = sorted(words, key=len)
print(sorted_words) # ['apple', 'cherry', 'banana']
```

Alternatively, you can use the "sort()" method of lists, which sorts the list in place and returns None. The basic syntax is:

```python
list.sort(key=None, reverse=False)
```

The "key" and "reverse" parameters work the same way as with the "sorted()" function.

For example:

```python
# Sort a list of numbers in ascending order
numbers = [3, 1, 4, 2, 5]
numbers.sort()
print(numbers) # [1, 2, 3, 4, 5]

# Sort a list of strings in descending order
words = ['apple', 'banana', 'cherry']
words.sort(reverse=True)
print(words) # ['cherry', 'banana', 'apple']

# Sort a list of strings by length
words = ['apple', 'banana', 'cherry']
words.sort(key=len)
print(words) # ['apple', 'cherry', 'banana']
```

Note that the sort() method does not return a new list and modifies the original one

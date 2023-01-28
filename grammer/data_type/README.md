# List

A Python list is a built-in data type that stores a collection of items in a specific order. 
Lists are mutable, meaning that the elements of a list can be changed. 
Lists are also used to store multiple items in a single variable.

Here is an example of a simple list:

```python
fruits = ["apple", "banana", "orange", "grapes"]
```

In this example, 'fruits' is a list that contains four elements: "apple", "banana", "orange", "grapes". 
Lists are created by placing a sequence of items inside square brackets '[]', separated by commas.

You can access the elements of a list by specifying the index of the element you want to access. 
The index of the first element is 0, the second element is 1, and so on.

```python
print(fruits[0]) # "apple"
print(fruits[1]) # "banana"
print(fruits[2]) # "orange"
print(fruits[3]) # "grapes"
```

You can also use negative indexing to access elements from the end of the list.

```python
print(fruits[-1]) # "grapes"
print(fruits[-2]) # "orange"
```

You can also use slicing to access a range of elements from a list.

```python
print(fruits[1:3]) # ["banana", "orange"]
```

In the above example, it will return the elements at index 1 to 2, but not the element at index 3.

You can add an element to a list using the 'append()' method.

```python
fruits.append("pineapple")
print(fruits) # ["apple", "banana", "orange", "grapes", "pineapple"]
```

You can also insert an element at a specific position using the insert() method.

```python
fruits.insert(1, "strawberry")
print(fruits) # ["apple", "strawberry", "banana", "orange", "grapes", "pineapple"]
```

You can remove an element from a list using the remove() method.

```python
fruits.remove("banana")
print(fruits) # ["apple", "strawberry", "orange", "grapes", "pineapple"]
```

You can also remove the last element from a list using the pop() method.

```python
fruits.pop()
print(fruits) # ["apple", "strawberry", "orange", "grapes"]
```

You can also use the len() function to find the number of elements in a list.

```python
print(len(fruits)) # 4
```

You can also use + operator to concatenate two lists.

```python
vegetables = ["carrot", "potato"]
all_items = fruits + vegetables
print(all_items) # ["apple", "strawberry", "orange", "grapes", "carrot", "potato"]
```

You can also use * operator to repeat the elements of a list.

```python
repeated_fruits = fruits * 2
print(repeated_fruits) # ["apple", "strawberry",
```


# Tuple

A Python tuple is a built-in data type that stores a collection of items in a specific order, similar to a list. 
However, unlike lists, tuples are immutable, meaning that the elements of a tuple cannot be changed once they are created.

Here is an example of a simple tuple:

```python
coords = (3, 4)
```

In this example, coords is a tuple that contains two elements: 3 and 4. Tuples are created by placing a sequence of items inside parentheses (), separated by commas.

You can access the elements of a tuple by specifying the index of the element you want to access, just like in a list.

```python
print(coords[0]) # 3
print(coords[1]) # 4
```

You can also use negative indexing and slicing to access elements from the end of the tuple or a range of elements from a tuple.

```python
print(coords[-1]) # 4
print(coords[1:]) # (4,)
```

You can unpack the tuple into separate variables by using the assignment operator.

```python
x, y = coords
print(x) # 3
print(y) # 4
```

You can use the len() function to find the number of elements in a tuple, just like in a list.

```python
print(len(coords)) # 2
```

You can also use + operator to concatenate two tuples.

```python
coords2 = (5,6)
concatenated_coords = coords + coords2
print(concatenated_coords) # (3, 4, 5, 6)
```

You can also use * operator to repeat the elements of a tuple.

```python
repeated_coords = coords * 3
print(repeated_coords) # (3, 4, 3, 4, 3, 4)
```

It's worth noting that tuples are less frequently used than lists in Python, but in certain cases like when you want to use a collection of items that will never change, it's a good choice to use tuples, because they are more memory-efficient than lists and also when you want to use as a key in a dictionary, since lists are not hashable.


# Dictionary

A Python dict (short for "dictionary") is a built-in data type that stores a collection of key-value pairs. Each key is associated with a value, and you can use the key to access the value. Dictionaries are also known as associative arrays or hash maps.

Here is an example of a simple dict:

```python
student = {'name': 'John Doe', 'age': 25, 'courses': ['Math', 'Physics']}
```

In this example, student is a dict that contains three key-value pairs:

* 'name': 'John Doe'
* 'age': 25
* 'courses': ['Math', 'Physics']

You can access the values of a dict by specifying the key you want to access, like this:

```python
print(student['name']) # 'John Doe'
print(student['courses']) # ['Math', 'Physics']
```

You can also use the get() method to access the value of a key. This method is useful when you want to provide a default value if the key is not found.

```python
print(student.get('name')) # 'John Doe'
print(student.get('address', 'Not found')) # 'Not found'
```

You can add a new key-value pair to a dict by using the assignment operator and specifying a new key, like this:

```python
student['address'] = '123 Main St'
```

You can remove a key-value pair from a dict by using the del statement and specifying the key, like this:

```python
del student['address']
```

You can use the keys() method to get a list of all the keys in a dict, and the values() method to get a list of all the values in a dict.

```python
print(student.keys()) # ['name', 'age', 'courses']
print(student.values()) # ['John Doe', 25, ['Math', 'Physics']]
```

You can use the items() method to get a list of all the key-value pairs in a dict, it returns the list of tuple containing key and value.

```python
print(student.items()) # [('name', 'John Doe'), ('age', 25), ('courses', ['Math', 'Physics'])]
```

You can also use in operator to check whether a key is present in a dict or not.

```python
print('name' in student) # True
print('address' in student) # False
```

Dictionaries are used to store a collection of items where each item has a unique label, the key, that can be used to access it. They are also commonly used for creating lookup tables and for storing data in a more organized way than lists or sets.

In Python, a class is a blueprint for creating objects (i.e. instances) with a certain set of attributes and methods. A class defines a new data type, and objects created from a class are called instances of that class.

Here is an example of a simple class called 'Person':

```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def say_hello(self):
        print("Hello, my name is " + self.name)

p = Person("John Doe", 30)
p.say_hello() # "Hello, my name is John Doe"
```

In the above example, Person is the name of the class. '__init__' is a special method that is called when an instance of the class is created. 
This method is used to initialize the attributes of the class. 
In this example, the '__init__' method takes two parameters name and age and assigns them to the attributes 'self.name' and 'self.age' respectively.

'say_hello' is a function of the class. 
It is used to define the behavior of the class. In this example, it prints a message with the name of the person.

'p = Person("John Doe", 30)' creates an instance of the class Person with the name "John Doe" and the age 30. 
And then we call the function 'say_hello()' on the created object which print the message.

You can also define class variables and class methods which are shared among all the instances of the class.

```python
class Person:
    count = 0
    def __init__(self, name, age):
        self.name = name
        self.age = age
        Person.count += 1

    def say_hello(self):
        print("Hello, my name is " + self.name)

    @classmethod
    def how_many(cls):
        print("Number of Person instances created: ", cls.count)

p1 = Person("John Doe", 30)
p2 = Person("Jane Doe", 25)
p1.say_hello() # "Hello, my name is John Doe"
p2.say_hello() # "Hello, my name is Jane Doe"
Person.how_many() # "Number of Person instances created: 2"
```

In this example, 'count' is a class variable which keeps track of the number of instances created. 
'how_many()' is a class method which can be called on the class and prints the number of instances created.

Python classes provide a way to organize and structure your code, making it easier to understand and maintain. 
They also allow you to create complex data structures and objects that can be used in various parts of your program.

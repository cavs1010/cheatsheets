# 🐍 Python Cheat Sheet 3 🐍

This cheatsheet covers key concepts in Python, including dictionaries, list comprehensions, and functions. We'll talk about what they are, how to use them, and include some handy examples. Let's get started! 👩‍💻

## Dictionaries 🗂️
A dictionary in Python is like a bag where you can put different things and each thing has a label attached to it. The label is called the 'key' and the thing itself is called the 'value'. 🏷️

~~~
# Creating a dictionary
my_dict = {'name': 'Alice', 'age': 20}
~~~

You can store any type of value in a dictionary. It could be a number, a string, a list, or even another dictionary (known as a nested dictionary)! 📚

To access a value in the dictionary, use its key:

~~~
print(my_dict['name'])  # Output: Alice
~~~

To change a value, also use its key:

~~~
my_dict['age'] = 21
print(my_dict['age'])  # Output: 21
~~~

#### Getting all the keys and values from a dictionary
~~~
# Here's our second example dictionary
my_dict = {"Alice": 25, "Bob": 30, "Charlie": 35}

# Get all keys
keys = my_dict.keys()
print(list(keys))  # Output: ['Alice', 'Bob', 'Charlie']

# Get all values
values = my_dict.values()
print(list(values))  # Output: [25, 30, 35]
~~~

#### Iterating Through a Dictionary with `.items()` 🔄

To get each key-value pair one by one, we use `.items()`. This is especially handy inside a `for` loop:

~~~
for key, value in my_dict.items():
    print(f"{key} is {value} years old.")
~~~

This will output:

~~~
Alice is 25 years old.
Bob is 30 years old.
Charlie is 35 years old.
~~~


## List Comprehensions 🔄
List comprehensions are like a magic spell that lets you make a whole list in just one line of code. 🪄

~~~
# Create a list of numbers 0-9
squares = [n for n in range(10)]
~~~

You can even change the items in the list or filter them:

~~~
# Create a list of odd squares
odd_squares = [n**2 for n in range(10) if n % 2 != 0]
~~~

## Functions 🧮
A function in Python is like a cooking recipe. 🍲 You give the recipe (function) some ingredients (parameters), and it will give you a dish (result).

~~~
def greet(name):
    print(f"Hello, {name}!")
~~~

Sometimes, a recipe can work even if you don't have all the ingredients. In a function, these are called default parameters.

~~~
def greet(name='Guest'):
    print(f"Hello, {name}!")
~~~

A function can also give you something back when it's done. This is called a return value.

~~~
def square(n):
    return n**2
~~~

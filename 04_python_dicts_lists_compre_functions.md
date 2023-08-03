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

Imagine list comprehension as a magic box 🎁 that takes in a list and transforms it into a new list. Here's how it works:

~~~
# This is our original list
original_list = [1, 2, 3, 4, 5]

# We give it to our magic box
new_list = [number * 2 for number in original_list]

# Let's see what our new list looks like
print(new_list)  # Output: [2, 4, 6, 8, 10]
~~~

In this example, our 'magic box' is doubling each number from the original list. The magic box is really just this line of code:

~~~
new_list = [number * 2 for number in original_list]
~~~

This says: "For each `number` in `original_list`, multiply `number` by 2 and put it into `new_list`." That's a list comprehension!

### Using `if` Statements in List Comprehensions 🚦

We can also use `if` statements inside our 'magic box'. Let's say we only want to double the numbers that are greater than 2:

~~~
# This is our original list again
original_list = [1, 2, 3, 4, 5]

# This time, we only double numbers greater than 2
new_list = [number * 2 for number in original_list if number > 2]

# Let's see the new list
print(new_list)  # Output: [6, 8, 10]
~~~

In this example, our 'magic box' only includes the numbers in the new list if they are greater than 2. 


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

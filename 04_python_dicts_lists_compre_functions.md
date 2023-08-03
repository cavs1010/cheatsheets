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
### Functions with No Parameters 🌮
Imagine you have a recipe to make a plain cheese quesadilla. You don't need to know anything extra; you just follow the recipe, and you'll get your cheese quesadilla.

In Python, a function without parameters is like this recipe. You don't need to give it any extra information; you just call the function, and it does its job.

~~~
def make_cheese_quesadilla():
    print("Cheese quesadilla is ready!")

make_cheese_quesadilla()  # This will print: Cheese quesadilla is ready!
~~~

### Functions with Parameters 🧀🍅
Now, what if you want to add some extra ingredients, like tomatoes or onions? You need to know which extras to add.

In Python, a function with parameters is like a customizable quesadilla recipe. You tell the function what you want, and it gives you a quesadilla with those specific ingredients.

~~~
def make_custom_quesadilla(cheese, filling):
    print(f"Quesadilla with {cheese} cheese and {filling} is ready!")

make_custom_quesadilla("Cheddar", "Tomatoes")  # This will print: Quesadilla with Cheddar cheese and Tomatoes is ready!
~~~

### Functions with Default Parameters 🧀🍅🌶️
Let's say that most of the time, you prefer cheddar cheese and chicken in your quesadilla, but you sometimes want to change it. 

You can have a default parameter in your function for these common ingredients, and change them when you want something different.

~~~
def make_default_quesadilla(cheese="Cheddar", filling="Chicken"):
    print(f"Quesadilla with {cheese} cheese and {filling} is ready!")

make_default_quesadilla()  # This will print: Quesadilla with Cheddar cheese and Chicken is ready!
make_default_quesadilla("Mozzarella", "Mushrooms")  # This will print: Quesadilla with Mozzarella cheese and Mushrooms is ready!
~~~

### Functions that Change a Variable 🔄
Imagine you have a pre-made quesadilla and want to add some hot sauce. You can modify the existing quesadilla, but your original recipe remains the same.

~~~
def add_hot_sauce(quesadilla):
    quesadilla += " with hot sauce"
    print(quesadilla)

quesadilla = "Chicken quesadilla"
add_hot_sauce(quesadilla)  # This will print: Chicken quesadilla with hot sauce
print(quesadilla)  # This will print: Chicken quesadilla (original variable is unchanged)
~~~

### Functions that Return a Value 🎁
Sometimes, you might want to keep the new customized quesadilla for later. A function that returns a value lets you store the result and use it elsewhere.

~~~
def add_guacamole(quesadilla):
    return quesadilla + " with guacamole"

quesadilla = "Beef quesadilla"
new_quesadilla = add_guacamole(quesadilla)  # You can keep this new quesadilla and use it later
print(new_quesadilla)  # This will print: Beef quesadilla with guacamole
~~~

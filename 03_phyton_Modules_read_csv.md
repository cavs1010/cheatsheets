# 🐍 Python Cheat Sheet 🐍

This cheat sheet covers reading, writing, appending to files, finding files with a relative path, importing modules, and provides a basic introduction to the string, random, os (with os.path.join), and csv modules.

## Reading Files 📖

To read a file in Python, you can use the `open` function along with the `read` method:

~~~
with open('myfile.txt', 'r') as file:
    content = file.read()
print(content)
~~~

## Writing to Files 🖊️

To write to a file in Python, you can use the `open` function with 'w' mode:

~~~
with open('myfile.txt', 'w') as file:
    file.write('Hello, world!')
~~~

Note: This will overwrite any existing content in the file.

## Appending to Files ➕

To append to a file in Python, you can use the `open` function with 'a' mode:

~~~
with open('myfile.txt', 'a') as file:
    file.write('Hello, again!')
~~~

## Relative Paths 🗺️

A relative path refers to the location of a file relative to the current working directory (the folder where your Python script is running). For example:

~~~
with open('./folder/myfile.txt', 'r') as file:
    content = file.read()
print(content)
~~~

Here, `./folder/myfile.txt` is the relative path to the file. `./` represents the current directory, and `folder/myfile.txt` is the path to the file from there.

## Importing Modules 🧩
In Python, a module is like a toolbox 🧰. It's a file containing a set of functions or variables that you can include in your project. Think of it like a piece of code that someone else has written that you can use in your own programs. For example, the math module in Python contains lots of helpful tools for doing mathematical operations. You can use the tools in the module by importing it into your code.

To use a module in Python, you can import it using the `import` keyword:

~~~
import math
~~~

## Basic Modules in Python 🔧

### String

The string module contains a number of useful constants and classes for working with strings:

~~~
import string

print(string.ascii_letters)  # prints all ASCII letters (lowercase and uppercase)
~~~

### Random

The random module is used to generate random numbers:

~~~
import random

print(random.randint(1, 10))  # prints a random integer between 1 and 10
~~~

### OS

The os module provides a way of using operating system dependent functionality. The os.path.join function is used to join one or more path components intelligently:

~~~
import os

print(os.getcwd())  # prints the current working directory

new_path = os.path.join(os.getcwd(), 'new_folder')
print(new_path)  # prints the path to 'new_folder' within the current working directory
~~~

### CSV
#### 🗂️ CSV Format 🗂️

CSV stands for "Comma-Separated Values". It's a simple file format used to store tabular data, such as a spreadsheet or database 📊. Each line of the file is a data record. Each record consists of one or more fields, separated by commas. 

For example, consider a CSV file with the following content:

~~~
Name,Age,City
Alice,20,New York
Bob,30,Los Angeles
Charlie,25,Chicago
~~~

Here, the first line is the header, and the following lines are the data records. 📝


The csv module implements classes to read and write tabular data in CSV format. In the example below, we specify the delimiter as ',':

~~~
import csv

with open('file.csv', 'r') as file:
    reader = csv.reader(file, delimiter=',')
    for row in reader:
        print(row)  # prints each row of the CSV file
~~~

# 🐍 Python Cheat Sheet 🐍

This README file is a cheat sheet for Python, including variable types, printing statements, using `str()` for printing numbers, f-string, inputs and prompts, if/elif/else statements, lists, removing elements from a list, and loops.

## Variable Types 🧮

- **Integer**
  ~~~
  x = 5
  ~~~
- **Float**
  ~~~
  y = 7.5
  ~~~
- **String**
  ~~~
  name = 'John'
  ~~~
- **Boolean**
  ~~~
  is_active = True
  ~~~

## Print Statements 🖨️

- **Print a String**
  ~~~
  print('Hello, world!')
  ~~~

- **Print a Variable**
  ~~~
  x = 10
  print(x)
  ~~~

- **Print a Number as a String**
  ~~~
  x = 10
  print('The number is ' + str(x))
  ~~~

## F-strings (formatted string literals) 🎭

- **Include a variable inside a string**
  ~~~
  name = 'John'
  print(f'Hello, {name}!')
  ~~~

## Inputs and Prompts 🎛️

- **Get user input**
  ~~~
  name = input('Enter your name: ')
  ~~~

## If/Elif/Else Statements 🚦

- **If statement**
  ~~~
  x = 10
  if x > 5:
      print('x is greater than 5')
  ~~~

- **If/Else statement**
  ~~~
  x = 3
  if x > 5:
      print('x is greater than 5')
  else:
      print('x is not greater than 5')
  ~~~

- **If/Elif/Else statement**
  ~~~
  x = 5
  if x > 5:
      print('x is greater than 5')
  elif x < 5:
      print('x is less than 5')
  else:
      print('x is equal to 5')
  ~~~

## Lists 📝

- **Create a list**
  ~~~
  numbers = [1, 2, 3, 4, 5]
  ~~~

- **Access a list item**
  ~~~
  first_number = numbers[0]
  ~~~

- **Add an item to a list**
  ~~~
  numbers.append(6)
  ~~~

- **Remove an item from a list**
  ~~~
  numbers.remove(1) # removes the first occurrence of 1 in the list
  ~~~

- **Remove an item at a specific index**
  ~~~
  numbers.pop(0) # removes the item at index 0
  ~~~

## Loops 🔄

- **For loop**
  ~~~
  numbers = [1, 2, 3, 4]
  for number in numbers:
      print(number) # it will print each of the elements in the list numbers
  ~~~

- **For loop with range**
  ~~~
  for i in range(5): # gives i values from 0 to 4
      print(i)
  ~~~

- **While loop**
  ~~~
  i = 0
  while i < 5:
      print(i)
      i += 1
  ~~~

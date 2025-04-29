# Python
Python is an interpreted, object-oriented, high-level programming lanaguage with dynamic semnatics. 

Usage:
- Software development (e.g. Developing a website with the Flask library)
- Data science (e.g. Creating a machine learning model with Tensorflow)
- Automation (e.g. Creating a script to automate data analysis using Excel)
Websites using python and django
- Youtube
- Instagram
- Spotify
- Dropbox
- Pinterest


## Naming Conventions

**Class** names should follow the CapWords convention.

For example: MyDog

**Function** names should be in all lowercase and underscores should be used to seperate words if necessary. 

```python 
def calculate_force(mass, acc):
    force = mass * acc
    return force
```

## Indentation

- Indentation groups lines of codes together. There should be 4 spaces per indentation. Spaces are preferred over tabs when making indentations. 

- You have to use the same number of spaces in the same block of code, otherwise Python will give you an error.

example: 
def calculate_force(mass, acc):
    force = mass * acc
    return force

## Comments 
There are blocks comments and inline comments. 

Block comments are used when there are multiple lines of comments.

Inline comments should be used when we have a short comment that we would like to include within a line of code.

Or you can use multiline string literals because they are not assigned to a variable.
```python
"""
This 
Is A
Multi-Line 
Comment
"""
```

# Command Line 

To run a program type the following:
python version & python file name
example: python myscript.py


# Variables 

We use variable to temporarily store data in computer's memory.
- In python variables are created when you assign a value to it.
- Python has NO command for declaring a variable. 
- Variables do not need to be declared with any particular type, and can even change type after they have been set.

*Rules for python variables*
- A variable name must start with a letter or the underscore character
- A variable name cannot start with a number
- A variable name can only contain alpha-numeric characters and underscores (A-z, 0-9, and _ )
- Variable names are case-sensitive (age, Age and AGE are three different variables)
- A variable name cannot be any of the Python keywords.
- Normally, when you create a variable inside a function, that variable is local, and can only be used inside that function.
- To create a global variable inside a function, you can use the global keyword.

Example:
```python 
myvar = "John"
my_var = "John"
_my_var = "John"
myVar = "John"
MYVAR = "John"
myvar2 = "John"
```
*Many Values to Multiple Variables*
Python allows you to assign values to multiple variables in one line.
*Many Values to Multiple Variables*
And you can assign the same value to multiple variables in one line.

### Casting 
If you want to specify the data type of a variable, this can be done with casting.

x = str(3)
y = int(3)
z = float(3)

### Get the Type
You can get the data type of a variable with the type() function.

```python 
x = 5
y = "John"
print(type(x))
print(type(y))
```

## Output 

- The best way to output multiple variables in the print() function is to separate them with commas, which even support different data


## Practice
- What is a correct syntax to add the value 'Hello World', to 3 variables in one statement?
x = y = z = 'Hello World'
- Insert the correct syntax to assign values to multiple variables in one line:
x,y,z = "Orange", "Banana", "Cherry"

# Python Collections (Arrays)
- List is a collection which is ordered and changeable. Allows duplicate members.
- Tuple is a collection which is ordered and unchangeable. Allows duplicate members.
- Set is a collection which is unordered, unchangeable*, and unindexed. No duplicate members.
- Dictionary is a collection which is ordered** and changeable. No duplicate members.
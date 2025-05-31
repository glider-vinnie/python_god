<h1> Introduction to Python </h1>
<h3>What is Python?</h3>
1. A high-level language, used in web development, data science, automation, AI, and more.<br>
2. Known for its readability, which means code is easier to write, understand, and maintain.<br>
3. Backed by library support, so you don’t have to build everything from scratch; there’s probably a library that already does what you need.<br>

<h3>Features of Python</h3>
1. Python requires fewer lines of code compared to other programming languages.<br>
2. Python is in high demand as it provides many job opportunities in Software Development, Data Science, and AI/ML.<br>
3. Python provides popular Web Development, AI/ML, Data Science, and Data Analysis Libraries like Django, Flask, Pandas, TensorFlow, Scikit-learn, and many more.<br>
4. Python is an object-oriented programming language which encapsulates code within objects.<br>
5. Python is cross-platform, working on Windows, Mac, and Linux without major changes.<br>
6. Python is used by big companies like Google, Netflix, and NASA.<br>
<h2> Installation </h2>
Visit the Python Software Foundation website at python.org. Any version of Python can be downloaded from there.<br>

<h4>Your First Python Program: The Classic</h4>
print("Hello World")<br>

<h3>Python Indentation</h3>
Indentation refers to the spaces at the beginning of a code line.
Where in other programming languages the indentation in code is for readability only, the indentation in Python is very important.
Python uses indentation to indicate a block of code.

<h3>Comments</h3>
Comments can be used to explain Python code.
Comments can be used to make the code more readable.
Comments can be used to prevent execution when testing code.
<h2>Creating a Comment</h2>
Comments starts with a #, and Python will ignore them.
Comments can be placed at the end of a line, and Python will ignore the rest of the line:

Example
print("Hello, World!") #This is a comment.
To add a multiline comment you could insert a # for each line or,
triple quotes """ ...
                  ...
                  ... """

<h3>Variables</h3>
Variables are containers for storing data values.
example: 
x = 5
y = "John"
print(x)
print(y)

<h2>Casting</h2>
If you want to specify the data type of a variable, this can be done with casting.
Example
x = str(3)    # x will be '3'
y = int(3)    # y will be 3
z = float(3)  # z will be 3.0
You can get the data type of a variable with the type() function.

<h2>Rules for Python variables:</h2>
A variable name must start with a letter or the underscore character
A variable name cannot start with a number
A variable name can only contain alpha-numeric characters and underscores (A-z, 0-9, and _ )
Variable names are case-sensitive (age, Age and AGE are three different variables)
A variable name cannot be any of the Python keywords.

Python allows you to assign values to multiple variables in one line:
Example: 
x, y, z = "Orange", "Banana", "Cherry"
One Value to Multiple Variables: x = y = z = "Orange"

<h4>Unpack a Collection</h4>
If you have a collection of values in a list, tuple etc. Python allows you to extract the values into variables. This is called unpacking.
Example
Unpack a list:
fruits = ["apple", "banana", "cherry"]
x, y, z = fruits
print(x)
print(y)
print(z)

<h3>Global Variables</h3>
Variables that are created outside of a function (as in all of the examples in the previous pages) are known as global variables.
Global variables can be used by everyone, both inside of functions and outside.
To create a global variable inside a function, you can use the global keyword.

<h2>Data types</h2>
Python has the following data types built-in by default, in these categories:

Text Type:	str
Numeric Types:	int, float, complex
Sequence Types:	list, tuple, range
Mapping Type:	dict
Set Types:	set, frozenset
Boolean Type:	bool
Binary Types:	bytes, bytearray, memoryview
None Type:	NoneType

<h3>String slicing</h3>

You can return a range of characters by using the slice syntax.
Specify the start index and the end index, separated by a colon, to return a part of the string.
b = "Hello, World!"
print(b[2:5])

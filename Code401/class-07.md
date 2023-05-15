# class_07

By diving into these topics and examples, Python developers can enhance their problem-solving abilities, write more efficient code,
and gain a deeper understanding of fundamental concepts that underlie many programming tasks. This knowledge empowers developers to 
tackle complex challenges, optimize performance, and ultimately deliver high-quality Python applications.

1. 
1. Variable scope in Python refers to the region or context in which a variable is visible and can be accessed. 
It determines where a variable can be used and how long it exists during the execution of a program. In Python, 
there are mainly two types of variable scope: local scope and global scope.

Local Scope:
Variables defined within a function have local scope and are only accessible within that function.
Local variables are created when the function is called and destroyed when the function exits.
Local variables cannot be accessed outside of the function.
Each function call creates a new instance of local variables, so different function calls can have separate local variables with the same name.
```python
def my_function():
    x = 10  # Local variable
    print(x)

my_function()  # Output: 10
print(x)  # Error: NameError: name 'x' is not defined
```
2. Global Scope:
Variables defined outside of any function or at the top level of a module have global scope.
Global variables are accessible throughout the entire module or program.
Global variables can be accessed and modified from both inside and outside of functions.
Global variables persist until the program execution ends or they are explicitly modified.

```python
x = 10  # Global variable

def my_function():
    print(x)  # Accessing global variable

my_function()  # Output: 10
print(x)  # Output: 10

def another_function():
    global x  # Declaring x as global
    x = 20  # Modifying global variable

another_function()
print(x)  # Output: 20
```

2.
Enclosing Scope: Also known as the non-local scope, it refers to the scope of variables in nested functions.
It allows inner functions to access variables from the outer function.

Global Scope: Variables defined at the top level of a module or declared as global inside a function have global scope. 
They can be accessed throughout the module or function, including nested functions.

3.
Big O notation is a way to describe the efficiency or complexity of an algorithm by analyzing how its execution time or space requirements
scale with input size. It provides a standardized notation to compare and classify algorithms based on their performance characteristics.

The purpose of Big O notation in algorithm analysis is to understand and predict how an algorithm will behave as the size of the input grows.
It helps us evaluate the scalability and efficiency of algorithms, allowing us to make informed decisions when selecting or designing algorithms 
for different tasks.


4.
using the random module
```python
import random
print(random.randint(1,6))
```



## Things I want to know more about

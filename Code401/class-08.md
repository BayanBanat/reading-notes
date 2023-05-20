# Class 08

 list comprehensions and decorators play a crucial role in writing clean, concise, and efficient code.
**Reading Questions:**
1.
* List comprehensions provide a concise way to create lists by performing operations on each element of an iterable. They are often more readable and compact compared to traditional for loops.
* The basic syntax of Python list comprehension is:
```python
[expression for item in iterable if condition]
```
* example of a list comprehension that squares the elements in a given list of integers:

```python
numbers = [1, 2, 3, 4, 5]
squared_numbers = [num ** 2 for num in numbers]
print(squared_numbers)
```
```Output:[1, 4, 9, 16, 25]```
2.
* Decorators are a powerful feature in Python that allow you to modify or enhance the behavior of functions or classes without directly changing their source code.
* Decorators provide a way to wrap or decorate functions or classes with additional functionality. They are implemented using the @decorator_name syntax or by manually applying the decorator using the decorator_name(original_function) syntax.
3.
how decorators work:

* Higher-Order Functions: In Python, functions are first-class objects, which means they can be assigned to variables, passed as arguments to other functions, and returned as values from other functions. This feature enables the use of higher-order functions, which are functions that can accept other functions as arguments or return functions.

* Decorator Function: A decorator is a higher-order function that takes a function as input, adds some functionality to it, and returns a modified or enhanced function. The decorator function typically defines an inner function that wraps or replaces the original function, adding extra behavior before or after its execution.

* Applying a Decorator: There are two ways to apply a decorator to a function or class. The most common and convenient way is using the @decorator_name syntax directly above the function or class definition. This syntax automatically applies the decorator to the function or class. Alternatively, you can manually apply the decorator using the decorator_name(original_function) syntax.

* Function Composition: Applying a decorator to a function effectively performs function composition. The decorator function wraps or replaces the original function with a new function that incorporates the desired enhancements or modifications.

Common use cases for decorators include:

* Logging
* Timing
* Authorization/Authentication
* Validation

example of a simple decorator function:
```python
import functools
import time

def timer(func):
    """Print the runtime of the decorated function"""
    @functools.wraps(func)
    def wrapper_timer(*args, **kwargs):
        start_time = time.perf_counter()    # 1
        value = func(*args, **kwargs)
        end_time = time.perf_counter()      # 2
        run_time = end_time - start_time    # 3
        print(f"Finished {func.__name__!r} in {run_time:.4f} secs")
        return value
    return wrapper_timer

@timer
def waste_some_time(num_times):
    for _ in range(num_times):
        sum([i**2 for i in range(10000)])
```


## Things I want to know more about
Decorators

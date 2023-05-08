# Class 4

Understanding Classes and Objects, Thinking Recursively, Pytest Fixtures, and Coverage is essential because they are fundamental concepts and tools that help developers write efficient, maintainable, and scalable code.

Classes and Objects provide a way to organize code into reusable and modular structures, making it easier to manage and extend.
Thinking Recursively is an important skill for developers to have because it allows them to break down complex problems into smaller, more manageable parts.
Fixtures provide a way to set up and tear down test environments, ensuring that tests are run in a consistent and controlled manner. This helps developers catch bugs and Errors early in the development process, leading to more robust and reliable code.
By increasing code coverage, developers can reduce the likelihood of bugs and errors in production, leading to a better user experience and more satisfied customers.


**Reading Questions :**

1- 

- A class is a template for creating objects, while an object is an instance of a class
- Classes define the attributes and methods that objects of that class will have, while objects are individual instances of the class that can be created and              manipulated.
     
Example of how classes and objects can be used to create and manage instances of a class:
  ```
class Person:
 def __init__(self, name, age):
    self.name = name
    self.age = age
        
 def introduce(self):
    print("Hi, my name is " + self.name + " and I am " + str(self.age) + " years old.")

# create objects of the Person class
person1 = Person("A", 25)
person2 = Person("B", 30)


# call object methods
person1.introduce()  # Output: Hi, my name is A and I am 25 years old.
```

2- 

- Recursion is a technique in programming where a function calls itself in order to solve a problem
- example of how recursion can be used to solve a problem in Python:
```
def factorial(n):
    if n == 1:
        return 1
    else:
        return n * factorial(n-1)
```
- The best practices to follow:
    - Define a base case.
    - Break down the problem.
    - Test thoroughly.
    
3- 

- Fixtures are functions that provide reusable test data or set up the test environment. They are defined using the @pytest.fixture decorator and can be called from     tests using the fixture name as a parameter. Fixtures can be used to set up database connections, create test data, or configure third-party libraries.
  By increasing code coverage, developers can reduce the likelihood of bugs and errors in production, leading to a better user experience and more satisfied customers.
- how they can be used together to improve the quality and maintainability of a project:
    - Reduce code duplication.
    - Improve test coverage.
    


  

## Things I want to know more about:

- Pytest Fixtures and Coverage

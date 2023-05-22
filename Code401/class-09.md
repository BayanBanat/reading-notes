# Read: Class 09


## Reading Questions
1. Dunder methods, also known as magic methods or special methods, are predefined methods in Python that start and end with double underscores.
    These methods allow you to define specific behaviors for built-in operations and language constructs. They are automatically called by Python
    in response to certain events or operations, providing a way to customize the behavior of objects.
```python
class Account:
    """A simple account class"""

    def __init__(self, owner, amount=0):
        """
        This is the constructor that lets us create
        objects from this class
        """
        self.owner = owner
        self.amount = amount
        self._transactions = []
```
2. The main ethical issue raised is plagiarism or unauthorized use of code or content created by developers without giving proper credit or compensation
     To avoid such ethical issues, there are several best practices that can be followed:
     * Respect intellectual property
     * Use open-source licenses
     * Collaborate transparently
     * Educate and promote ethical practices
3. The Python statistics module is a built-in module that provides a set of functions for performing various statistical calculations. 
   It is part of the Python Standard Library, starting from Python 3.4. The module offers a convenient way to work with statistical data 
   and perform common operations such as calculating measures of central tendency, dispersion, correlation, and more.
   
```python
import statistics

data = [2, 4, 6, 8, 10]

mean = statistics.mean(data)
print(mean)
```

## Things I want to know more about
Statistics

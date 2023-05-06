# FileIO & Exceptions

Python provides a simple and powerful way to **read** and **write** files using the built-in **open()** function and file objects.
Being able to read and write files allows developers to access and manipulate data stored in files, which can be used
to build more powerful and flexible applications.
The ability to read and write files in Python, and the understanding of how to handle exceptions, are important skills for web developers to have, 
as they enable them to build more powerful, flexible, and resilient web applications.

### Reading Questions:

It's important to note that when you open a file, you should always close it when you're done working with it to free up system resources. 
in this you can use the **with** statement to automatically close the file when you're finished in a safe and efficient way which helps prevent 
data corruption and other problems.
like this:
```
with open('abc.txt', 'r') as file:
    data = file.read()
    
```

The read() method reads the entire contents of a file into a single string. This method can be useful when you need to read the entire
file at once and perform operations on the contents as a whole **is best suited for reading small files or when you need to read the entire file at once**.
like this:
```
with open('abc.txt', 'r') as file:
    data = file.read()
```

The readline() method, on the other hand, reads a single line of text from the file. This method can be useful when you need to read a file 
line by line and perform operations on each line individually **is best suited for reading large files or when you need to read the file line by line**.
like this:
```
with open('abc.txt', 'r') as file:
    line = file.readline()
    while line:
        print(line)
        line = file.readline()     
```


**Exceptions** are a mechanism in Python for handling errors that occur during the execution of a program. When an error occurs, an exception is raised,
which can be caught and handled by the program and it allows us to handle errors or unexpected situations that may occur during program execution.
like this:

```
try:
    num = int(input("Enter a number: "))
    print(10 / num)
except ZeroDivisionError:
    print("Cannot divide by zero.")
except ValueError:
    print("Please enter a valid integer.")
finally:
    print("Thank you for using this program.")
    
```

## Things I want to know more about:

- Exceptions
- Line Endings



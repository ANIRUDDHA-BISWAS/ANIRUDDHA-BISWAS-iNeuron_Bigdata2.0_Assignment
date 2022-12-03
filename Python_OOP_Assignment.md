Q1. What is the purpose of Python's OOP?<br>
Ans. OOPS is abbreviated as Object Oriented Programming system in which programs are considered as a collection of objects. Each object is nothing but an instance of a class.<br>
OOP is about code reuse — you factor code to minimize redundancy and program by customizing what already exists instead of changing code in place or starting from scratch.

Q2. Where does an inheritance search look for an attribute?<br>
Ans. An inheritance search looks for an attribute first in the instance object, then in the class the instance was created from, then in all higher superclasses, progressing from left to right (by default). The search stops at the first place the attribute is found.

Q3. How do you distinguish between a class object and an instance object?<br>
Ans. Classes are a kind of factory for creating multiple instances. Classes also support operator overloading methods, which instances inherit, and treat any functions nested in the class as methods for processing instances.

Q4. What makes the first argument in a class’s method function special?<br>
Ans. It always receives the instance object that is the implied subject of the method call. It’s usually called 'self' by convention.

Q5. What is the purpose of the init method?<br>
Ans. If the __init__ method is coded or inherited in a class, Python calls it automatically each time an instance of that class is created.

Q6. What is the process for creating a class instance?<br>
Ans. You create a class instance by calling the class name as though it were a function; any arguments passed into the class name show up as arguments two and beyond in the __init__ constructor method.

Q7. What is the process for creating a class?<br>
Ans. In Python, Use the keyword class to define a Class. In the class definition, the first string is docstring which, is a brief description of the class.
The docstring is not mandatory but recommended to use. We can get docstring using __doc__ attribute. Use the following syntax to create a class.

Q8. How would you define the superclasses of a class?<br>
Ans. The class from which a class inherits is called the parent or superclass. A class which inherits from a superclass is called a subclass, also called heir class or child class. Superclasses are sometimes called ancestors as well.

Q9. What is the relationship between classes and modules?<br>
Ans. The difference between a class and a module in python is that a class is used to define a blueprint for a given object, whereas a module is used to reuse a given piece of code inside another program.

Q10. How do you make instances and classes?<br>
Ans:Everything in Python is an object such as integers, lists, dictionaries, functions and so on. Every object has a type and the object types are created using classes. Instance is an object that belongs to a class. For instance, list is a class in Python.<br>
To create instances of a class, we call the class using class name and pass in whatever arguments its __init__ method accepts.

Q11. Where and how should be class attributes created?<br>
Ans:The attribute defined in the class is called “class attributes’ and the attributes defined in the function is called ‘instance attributes’. While defining, these attributes are not prefixed by self, as these are the property of the class and not of a particular instance.<br>
The class attributes can be accessed by the class itself ( className.attributeName) as well as by the instances of the class (inst.attributeName). So, the instances have access to both the instance attribute as well as class attributes.<br>
A class attribute can be overridden in an instance, even though it is not a good method to break encapsulation.

Q12. Where and how are instance attributes created?<br>
Ans:Instance Attributes are unique to each object, (an instance is another name for an object). Here, any Dog object we create will be able to store its name and age. We can change either attribute of either dog, without affecting any other dog objects we've created.<br>
We add instance attributes usually by defining the constructor method “__init__”. Within __init__ we pass the first parameters self which represents an object from a class that is currently being defined, and usually, we attach instance attributes to these objects using the dot operator.

Q13. What does the term "self" in a Python class mean?<br>
Ans: The self is used to represent the instance of the class. With this keyword, we can access the attributes and methods of the class in python. It binds the attributes with the given arguments. The reason why we use self is that Python does not use the ‘@’ syntax to refer to instance attributes. In Python, we have methods that make the instance to be passed automatically, but not received automatically.

Q14. How does a Python class handle operator overloading?<br>
Ans: Python operators work for built-in classes. But the same operator behaves differently with different types. For example, the + operator will perform arithmetic addition on two numbers, merge two lists, or concatenate two strings.

This feature in Python that allows the same operator to have different meaning according to the context is called operator overloading.

Let us consider the following class, which tries to simulate a point in 2-D coordinate system.
```
class Point:
    def __init__(self, x=0, y=0):
        self.x = x
        self.y = y

p1 = Point(1, 2)
p2 = Point(2, 3)
print(p1+p2)
```
Output:<br>
Traceback (most recent call last):<br>
  File "<string>", line 9, in <module> <br>
    print(p1+p2)<br>
TypeError: unsupported operand type(s) for +: 'Point' and 'Point'<br>
Here, we can see that a TypeError was raised, since Python didn't know how to add two Point objects together.

Q15. When do you consider allowing operator overloading of your classes?<br>
Ans:The operator overloading in Python means provide extended meaning beyond their predefined operational meaning. Such as, we use the "+" operator for adding two integers as well as joining two strings or merging two lists. We can achieve this as the "+" operator is overloaded by the "int" class and "str" class.

Q16. What is the most popular form of operator overloading?<br>
Ans: A very popular and convenient example is the Addition (+) operator.<br>
Just think how the ‘+’ operator operates on two numbers and the same operator operates on two strings. It performs “Addition” on numbers whereas it performs “Concatenation” on strings.

Q17. What are the two most important concepts to grasp in order to comprehend Python OOP code?<br>
Ans:In order to develop robust and well-designed software products with Python, it is essential to obtain a comprehensive understanding of OOP. In this article, we will elaborate on two key concepts of OOP which are inheritance and polymorphism. Both inheritance and polymorphism are key ingredients for designing robust, flexible, and easy-to-maintain software. 

Q18. Describe three applications for exception processing.<br>
Ans:In Python, exceptions can be handled using a try statement.<br>
The critical operation which can raise an exception is placed inside the try clause. The code that handles the exceptions is written in the except clause.We can thus choose what operations to perform once we have caught the exception.<br>
Here is a simple example.
```
# import module sys to get the type of exception 
import sys

randomList = ['a', 0, 2]

for entry in randomList:
    try:
        print("The entry is", entry)
        r = 1/int(entry)
        break
    except:
        print("Oops!", sys.exc_info()[0], "occurred.")
        print("Next entry.")
        print()
print("The reciprocal of", entry, "is", r)
```
Output:<br>
The entry is a<br>
Oops! <class 'ValueError'> occurred.<br>
Next entry.<br>
	
The entry is 0<br>
Oops! <class 'ZeroDivisionError'> occured.<br>
Next entry.<br>

The entry is 2<br>
The reciprocal of 2 is 0.5<br>
In this program, we loop through the values of the randomList list. As previously mentioned, the portion that can cause an exception is placed inside the try block.If no exception occurs, the except block is skipped and normal flow continues(for last value). But if any exception occurs, it is caught by the except block (first and second values).Here, we print the name of the exception using the exc_info() function inside sys module. We can see that a causes ValueError and 0 causes ZeroDivisionError.
	

Q19. What happens if you don't do something extra to treat an exception?<br>
Ans:An exception object is created when a Python script raises an exception. If the script explicitly doesn't handle the exception, the program will be forced to terminate abruptly.

Q20. What are your options for recovering from an exception in your script?<br>
Ans:The try-catch is the simplest method of handling exceptions. Put the code you want to run in the try block, and any Java exceptions that the code throws are caught by one or more catch blocks. This method will catch any type of Java exceptions that get thrown. This is the simplest mechanism for handling exceptions.

Q21. Describe two methods for triggering exceptions in your script.<br>
Ans:To avoid such a scenario, there are two methods to handle Python exceptions: Try – This method catches the exceptions raised by the program. Raise – Triggers an exception manually using custom exceptions.

Q22. Identify two methods for specifying actions to be executed at termination time, regardless of whether or not an exception exists.<br>

Q23. What is the purpose of the try statement?<br>

Q24. What are the two most popular try statement variations?<br>

Q25. What is the purpose of the raise statement?<br>
Python raise Keyword is used to raise exceptions or errors. The raise keyword raises an error and stops the control flow of the program. It is used to bring up the current exception in an exception handler so that it can be handled further up the call stack.<br>
Example: In the below code, we check if an integer is even or odd. if the integer is odd an exception is raised.  a  is a variable to which we assigned a number 5, as a is odd, then if loop checks if it’s an odd integer, if it’s an odd integer then an error is raised.
```
a = 5

if a % 2 != 0:
	raise Exception("The number shouldn't be an odd integer")
```

Q26. What does the assert statement do, and what other statement is it like?<br>
Ans: Python has built-in assert statement to use assertion condition in the program. assert statement has a condition or expression which is supposed to be always true. If the condition is false assert halts the program and gives an AssertionError.

Q27. What is the purpose of the with/as argument, and what other statement is it like?<br>

Q28. What are *args, ***kwargs?

Ans. The special syntax *args in function definitions in python is used to pass a variable number of arguments to a function. It is used to pass a non-key worded, variable-length argument list.<br> 
The syntax is to use the symbol * to take in a variable number of arguments; by convention, it is often used with the word args.<br>
What *args allows you to do is take in more arguments than the number of formal arguments that you previously defined. With *args, any number of extra arguments can be tacked on to your current formal parameters (including zero extra arguments).<br>
For example, we want to make a multiply function that takes any number of arguments and is able to multiply them all together. It can be done using *args.<br>
Using the *, the variable that we associate with the * becomes an iterable meaning you can do things like iterate over it, run some higher-order functions such as map and filter, etc.<br>

The special syntax **kwargs** in function definitions in python is used to pass a keyworded, variable-length argument list. We use the name kwargs with the double star. The reason is that the double star allows us to pass through keyword arguments (and any number of them).<br>
A keyword argument is where you provide a name to the variable as you pass it into the function.<br>
One can think of the kwargs as being a dictionary that maps each keyword to the value that we pass alongside it. That is why when we iterate over the kwargs there doesn’t seem to be any order in which they were printed out.


Q29. How can I pass optional or keyword parameters from one function to another?<br>
Ans. To pass optional or keyword parameters from one function to another, collect the arguments using the * and ** specifiers in the function’s parameter list But, at first, do know what are *args and **args in Python.

Q30. What are Lambda Functions?<br>
Ans. Python Lambda Functions are anonymous function means that the function is without a name. As we already know that the def keyword is used to define a normal function in Python. Similarly, the lambda keyword is used to define an anonymous function in Python. 

Q31. Explain Inheritance in Python with an example?<br>
Ans. In Python, inheritance is the process of inheriting the properties of the parent class into a child class. The primary purpose of inheritance is the reusability of code. Using inheritance, we can use the existing class to create a new class instead of recreating it from scratch.<br>
In the below example, From a vehicle class, we are creating a Car class. We don't need to define common attributes and methods again in Car class. We only need to add those attributes and methods which are specific to the Car.<br>
In inheritance, the child class acquires all the data members, properties, and functions of the parent class. Also, a child class can customize any of the parent class methods.
```
# Base class
class Vehicle:

    def __init__(self, name, color, price):
        self.name = name
        self.color = color
        self.price = price

    def info(self):
        print(self.name, self.color, self.price)

# Child class
class Car(Vehicle):

    def change_gear(self, no):
        print(self.name, 'change gear to number', no)

# Create object of Car
car = Car('BMW X1', 'Black', 35000)
car.info()
car.change_gear(5)
```

Q32. Suppose class C inherits from classes A and B as class C(A,B).Classes A and B both have their own versions of method func(). If we call func() from an object of class C, which version gets invoked?<br>

Q33. Which methods/functions do we use to determine the type of instance and inheritance?<br>

Q34.Explain the use of the 'nonlocal' keyword in Python.<br>
The nonlocal keyword is used to work with variables inside nested functions, where the variable should not belong to the inner function. Use the keyword nonlocal to declare that the variable is not local.
```
#Make a function inside a function, which uses the variable x as a non local variable.
def myfunc1():
  x = "John"
  def myfunc2():
    nonlocal x
    x = "hello"
  myfunc2()
  return x

print(myfunc1())
```

Q35. What is the global keyword?<br>
Ans. The global keyword is used to create global variables from a no-global scope, e.g. inside a function.
```
# Declare a global variable inside a function, and use it outside the function.
#create a function:
def myfunction():
  global x
  x = "hello"

#execute the function:
myfunction()

#x should now be global, and accessible in the global scope.
print(x)
```




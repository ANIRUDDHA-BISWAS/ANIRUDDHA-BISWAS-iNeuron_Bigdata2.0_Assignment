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

Q11. Where and how should be class attributes created?<br>

Q12. Where and how are instance attributes created?<br>

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

Q16. What is the most popular form of operator overloading?<br>
Ans: A very popular and convenient example is the Addition (+) operator.<br>
Just think how the ‘+’ operator operates on two numbers and the same operator operates on two strings. It performs “Addition” on numbers whereas it performs “Concatenation” on strings.

Q17. What are the two most important concepts to grasp in order to comprehend Python OOP code?<br>

Q18. Describe three applications for exception processing.<br>

Q19. What happens if you don't do something extra to treat an exception?<br>

Q20. What are your options for recovering from an exception in your script?<br>

Q21. Describe two methods for triggering exceptions in your script.<br>

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




Q1. What is the purpose of Python's OOP?<br>
Ans. OOP is about code reuse — you factor code to minimize redundancy and program by customizing what already exists instead of changing code in place or starting from scratch.

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

Q8. How would you define the superclasses of a class?<br>

Q9. What is the relationship between classes and modules?<br>

Q10. How do you make instances and classes?<br>

Q11. Where and how should be class attributes created?<br>

Q12. Where and how are instance attributes created?<br>

Q13. What does the term "self" in a Python class mean?<br>

Q14. How does a Python class handle operator overloading?<br>

Q15. When do you consider allowing operator overloading of your classes?<br>

Q16. What is the most popular form of operator overloading?<br>

Q17. What are the two most important concepts to grasp in order to comprehend Python OOP code?<br>

Q18. Describe three applications for exception processing.<br>

Q19. What happens if you don't do something extra to treat an exception?<br>

Q20. What are your options for recovering from an exception in your script?<br>

Q21. Describe two methods for triggering exceptions in your script.<br>

Q22. Identify two methods for specifying actions to be executed at termination time, regardless of whether or not an exception exists.<br>

Q23. What is the purpose of the try statement?<br>

Q24. What are the two most popular try statement variations?<br>

Q25. What is the purpose of the raise statement?<br>

Q26. What does the assert statement do, and what other statement is it like?<br>

Q27. What is the purpose of the with/as argument, and what other statement is it like?<br>

Q28. What are *args, **kwargs?<br>

Q29. How can I pass optional or keyword parameters from one function to another?<br>

Q30. What are Lambda Functions?<br>

Q31. Explain Inheritance in Python with an example?<br>
Ans. In Python, inheritance is the process of inheriting the properties of the parent class into a child class. The primary purpose of inheritance is the reusability of code. Using inheritance, we can use the existing class to create a new class instead of recreating it from scratch.
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




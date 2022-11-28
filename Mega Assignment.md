## Assignment Part-1

Q1. Why do we call Python as a general purpose and high-level programming language?<br>
Ans: Python is one of the most popular and user-friendly programming languages out there.
It is an object-oriented, high-level programming language. Object-oriented means this language is based around objects (such as data) rather than functions, and high-level means it's easy for humans to understand.

Q2. Why is Python called a dynamically typed language?<br>
Ans: Other languages like C, C++, Java, etc. there is a strict declaration of variables before assigning values to them but Python doesn't have any problem even if we don't declare the type of variable. It states the kind of variable in the runtime of the program. Python also takes care of the memory management which is crucial in programming. So, Python is a dynamically typed language.

Q3. List some pros and cons of Python programming language?  
Ans: Pros and Cons of Python Programming Language -<br>
Pros:<br>
      Beginner-friendly, is easy to learn and read.<br>
      Python has a vast collection of libraries.<br>
      Python is free, open-source, and has a vibrant community.<br>
      Python is a portable programming language.<br>
      Python is an interpreted, Embeddable Highly Scalable language.<br>
Cons:<br>
      Python has speed limitations & High memory consumption.<br>
      Python has issues with design.<br>
      Slower than compiled languages.<br>
      Complex multithreading.<br>

Q4. In what all domains can we use Python?<br>
Ans:  Machine learning / Artificial intelligence.<br>
      Desktop GUI.<br>
      Data analytics and data visualization.<br>
      Web development.<br>
      Game development.<br>
      Mobile app development.

Q5. What are variable and how can we declare them?<br>
Ans: Python has no command for declaring a variable.
Thus, declaring a variable in Python is very simple.
Just name the variable & Assign the required value to it.
The data type of the variable will be automatically determined from the value assigned, we need not define it explicitly.

Q6. How can we take an input from the user in Python?<br>
Ans: In Python, Using the input() function, we take input from a user.<br>
```
# Example 
name=(input("Enter Your Name: "))
print("Hello ",name)
# Here "name" is use as a variable & "input" is a Python built in Function.
```

Q7. What is the default datatype of the value that has been taken as an input using input() function?<br>
Ans: String, everything that you input() will be a string as default.

Q8. What is type casting?<br>
Ans: The conversion of one data type into the other data type is known as type casting in python or type conversion in python.<br>
Python supports a wide variety of functions or methods like: int(), float(), str(), ord(), hex(), oct(), tuple(), set(), list(), dict(), etc. for the type casting in python.

Q9. Can we take more than one input from the user using single input() function? If yes, how? If no, why?<br>

Q10. What are keywords?<br>
Ans: Keywords are some predefined and reserved words in python that have special meanings. Keywords are used to define the syntax of the coding. The keyword cannot be used as an identifier, function and variable name.<br>
Example: if, elif, else, True, False etc.

Q11. Can we use keywords as a variable? Support your answer with reason.<br>
Ans: An example of something we can’t do with Python keywords is assign something to them. If we try, then we’ll get a SyntaxError. we won’t get a SyntaxError if we try to assign something to a built-in function or type, but it still isn’t a good idea. For a more in-depth explanation of ways keywords can be misused, check out Invalid Syntax in Python: Common Reasons for SyntaxError.

Q12. What is indentation? What's the use of indentaion in Python?<br>
Ans: Python indentation refers to adding white space before a statement to a particular block of code. In another word, all the statements with the same space to the right, belong to the same code block.<br>
Example of Python Indentation.

Q13. How can we throw some output in Python?<br>
Ans:The basic way to do output is the print statement. To end the printed line with a newline, add a print statement without any objects. This will print to any object that implements write(), which includes file objects.

Q14. What are operators in Python?<br>
Ans: In Python, operators are special symbols that designate that some sort of computation should be performed. The values that an operator acts on are called operands.<br>
Types of Python Operators:<br>
                        Arithmetic operators<br>
                        Assignment Operators<br>
                        Comparison Operators<br>
                        Logical Operators<br>
                        Bitwise Operators<br>
                        Special Operators<br>

Q15. What is difference between / and // operators?<br>
Ans: / (Division) Divides two numbers. It provides decimal places.<br>
// (Floor Division) Divides two numbers & removes the decimal place. But in case of Negative value it floors the number too far from zero.

Q16. Write a code that gives following as an output.
```
iNeuroniNeuroniNeuroniNeuron
```
```
name="iNeuron"
print(name*4)
# Here "name" is use as a variable & Arithmetic Operators * (Multiply) used.
```

Q17. Write a code to take a number as an input from the user and check if the number is odd or even.
```
a = int(input("Enter a Number: ")) 
if (a % 2 == 0): 
  print("The number is Even") 
else: 
  print("The number is Odd")
# Here "a" is use as a variable & IF Statement used.
```

Q18. What are boolean operator?<br>
Ans: Booleans are simple and easy to use concepts that exist in every programming language. A boolean represents an idea of “true” or “false.” While writing an algorithm or any program, there are often situations where we want to execute different code in different situations. Booleans help our code to do just that easy and effective. More often, a boolean value is returned as a result of some kind of comparison operations.
There are two Boolean keywords: True and False

Q19. What will the output of the following?
```
1 or 0

0 and 0

True and False and True

1 or 0 or 0
```

Q20. What are conditional statements in Python?<br>
Ans: Conditional Statement in Python perform different computations or actions depending on whether a specific Boolean constraint evaluates to true or false. Conditional statements are handled by IF statements in Python.

Q21. What is use of 'if', 'elif' and 'else' keywords?<br>
Ans: if… elif…else are conditional statements that provide you with the decision making that is required when you want to execute code based on a particular condition. The if… elif…else statement used in Python helps automate that decision making process.

Q22. Write a code to take the age of person as an input and if age >= 18 display "I can vote". If age is < 18 display "I can't vote".
```
a=int(input("Enter Your Age: "))
if a>=18:
   print("I can vote")
else:
   print("I can't vote")
# Here "a" is use as a variable & IF/Else Statement used.
```

Q23. Write a code that displays the sum of all the even numbers from the given list.
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```


Q24. Write a code to take 3 numbers as an input from the user and display the greatest no as output.

Q25. Write a program to display only those numbers from a list that satisfy the following conditions

- The number must be divisible by five

- If the number is greater than 150, then skip it and move to the next number

- If the number is greater than 500, then stop the loop
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```

Q26. What is a string? How can we declare string in Python?<br>
Ans: A string is a sequence of characters.
Strings can be created by enclosing characters generally inside a single quote or double-quotes. 

Q27. How can we access the string using its index?

Q28. Write a code to get the desired output of the following
```
string = "Big Data iNeuron"
desired_output = "iNeuron"
```

Q29. Write a code to get the desired output of the following
```
string = "Big Data iNeuron"
desired_output = "norueNi"
```

Q30. Resverse the string given in the above question.

Q31. How can you delete entire string at once?<br>
Ans: Python will not allow deleting a particular character in a string. Whereas you can remove the entire string variable using the del command.

Q32. What is escape sequence?<br>
Ans: An escape sequence is a sequence of characters that, when used inside a character or string, does not represent itself but is converted into another character or series of characters that may be difficult or impossible to express directly, like newline (\n), tab (\t), and so on.

Q33. How can you print the below string?
```
'iNeuron's Big Data Course'
```

Q34. What is a list in Python?<br>
Ans: List is a collection of different values or different types of items. Unlike array in c/c++/lava a List is capable of storing different types of values under one roof. The items in the list are separated with the comma (,) and enclosed with the square brackets[ ].
Provides us the facility to store multiple types of values in a single unit.

Q35. How can you create a list in Python?<br>
Ans: In Python, a list is created by placing elements inside square brackets [ ], separated by commas(,).

Q36. How can we access the elements in a list?<br>
Ans: To access values in lists, use the square brackets for slicing along with the index or indices to obtain value available at that index. For example −

Q37. Write a code to access the word "iNeuron" from the given list.
```
lst = [1,2,3,"Hi",[45,54, "iNeuron"], "Big Data"]
``` 

Q38. Take a list as an input from the user and find the length of the list.

Q39. Add the word "Big" in the 3rd index of the given list.
```
lst = ["Welcome", "to", "Data", "course"]
```

Q40. What is a tuple? How is it different from list?<br>
Ans: Tuples are used to store multiple items in a single variable.
Tuple is one of 4 built-in data types in Python used to store collections of data, the other 3 are List, Set, and Dictionary, all with different qualities and usage.
A tuple is a collection which is ordered and unchangeable.<br>
Differences between Tuple & list:  
i) List are mutable where Tuples are immutable<br>
ii) Iterations are time-consuming in List where Iterations are comparatively Faster in Tuple.<br>
iii) Inserting and deleting items is easier with a list where Accessing the elements is best accomplished with a tuple data type.<br>
iv) Lists consume more memory where Tuple consumes less than the list.<br>
v) Lists have several built-in methods where A tuple does not have many built-in methods because of immutability.<br>
vi) A unexpected change or error is more likely to occur in a list where In a tuple, changes and errors don't usually occur because of immutability.

Q41. How can you create a tuple in Python?<br>
Ans: A tuple is created by placing all the items (elements) inside parentheses (), separated by commas. The parentheses are optional, however, it is a good practice to use them.
A tuple can have any number of items and they may be of different types (integer, float, list, string, etc.).

Q42. Create a tuple and try to add your name in the tuple. Are you able to do it? Support your answer with reason.

Q43. Can two tuple be appended. If yes, write a code for it. If not, why?

Q44. Take a tuple as an input and print the count of elements in it.

Q45. What are sets in Python?

Q46. How can you create a set?

Q47. Create a set and add "iNeuron" in your set.

Q48. Try to add multiple values using add() function.

Q49. How is update() different from add()?

Q50. What is clear() in sets?

Q51. What is frozen set?

Q52. How is frozen set different from set?

Q53. What is union() in sets? Explain via code.

Q54. What is intersection() in sets? Explain via code.

Q55. What is dictionary ibn Python?

Q56. How is dictionary different from all other data structures.

Q57. How can we delare a dictionary in Python?

Q58. What will the output of the following?
```
var = {}
print(type(var))
```

Q59. How can we add an element in a dictionary?

Q60. Create a dictionary and access all the values in that dictionary.

Q61. Create a nested dictionary and access all the element in the inner dictionary.

Q62. What is the use of get() function?<br>
Ans: Python Dictionary get() Method return the value for the given key if present in the dictionary. If not, then it will return None (if get() is used with only one argument).

Q63. What is the use of items() function?<br>
Ans: In Python Dictionary, items() method is used to return the list with all dictionary keys with values.

Q64. What is the use of pop() function?<br>
Ans: Python dictionary pop() method removes and returns the specified element from the dictionary.

Q65. What is the use of popitems() function?<br>
Ans: Python dictionary popitem() method removes the last inserted key-value pair from the dictionary and returns it as a tuple.

Q66. What is the use of keys() function?<br>
Ans: The keys() method in Python Dictionary, returns a view object that displays a list of all the keys in the dictionary in order of insertion using Python.

Q67. What is the use of values() function?<br>
Ans: values() is an inbuilt method in Python programming language that returns a view object. The view object contains the values of the dictionary, as a list. If you use the type() method on the return value, you get “dict_values object”. It must be cast to obtain the actual list.

Q68. What are loops in Python?<br>
Ans: Looping statement is a control statement which keeps on executing a single statement or a block of statements "N" times till the condition is true. Once the condition becomes false the execution is terminated

Q69. How many type of loop are there in Python?<br>
Ans: There are two types of loops in Python, “for” and “while”.

Q70. What is the difference between for and while loops?<br>
Ans:

Q71. What is the use of continue statement?<br>
Ans: The continue statement is used to skip the rest of the code inside a loop for the current iteration only. Loop does not terminate but continues on with the next iteration.

Q72. What is the use of break statement?<br>
Ans:The break statement terminates the loop containing it. Control of the program flows to the statement immediately after the body of the loop.
If the break statement is inside a nested loop (loop inside another loop), the break statement will terminate the innermost loop.

Q73. What is the use of pass statement?<br>
Ans:In Python programming, the pass statement is a null statement which can be used as a placeholder for future code.
Suppose we have a loop or a function that is not implemented yet, but we want to implement it in the future. In such cases, we can use the pass statement.

Q74. What is the use of range() function?<br>
Ans: The Python range() function returns a sequence of numbers, in a given range. The most common use of it is to iterate sequence on a sequence of numbers using Python loops.

Q75. How can you loop over a dictionary?<br>
Ans:


### Coding problems
Q76. Write a Python program to find the factorial of a given number.
```
i=int(input("Enter Number: "))
fac=1
while (i>0):
    fac=fac*i
    i=i-1
print("Factorial =",fac)
```

Q77. Write a Python program to calculate the simple interest. Formula to calculate simple interest is SI = (P*R*T)/100
```
# print("The simple interset is: ",SimpleInterset)
def simple_interest(p,r,t):
    si = (p * r * t)/100
    return si
      
p=int(input("Enter Principal Amount: "))
r=float(input("Enter Rate of Interest: "))
t=int(input("Enter the number of Years: "))

print('The Simple Interest is', simple_interest(p, r, t))
```

Q78. Write a Python program to calculate the compound interest. Formula of compound interest is A = P(1+ R/100)^t.
```
import math  
def compound_interest(p,r,t):   
    amt = p * (math.pow((1 + (r/100)),t))
    print("Compound Amount: ",amt)
    CI = amt - p
    return CI

p=float(input("Enter Principal Amount: "))
r=float(input("Enter Rate of Interest: "))
t=float(input("Enter the number of Years: "))

print("Compound interest is",compound_interest(p,r,t))
```

Q79. Write a Python program to check if a number is prime or not.
```
n=int(input("Enter Number: "))
count=0
i=1
while (i<=n):
    if (n%i==0):
        count=count+1
    i=i+1
if(count==2):
    print("It's Prime Number")
else:
    print("It's Composite Number")
```

Q80. Write a Python program to check Armstrong Number.

Q81. Write a Python program to find the n-th Fibonacci Number.

Q82. Write a Python program to interchange the first and last element in a list.

Q83. Write a Python program to swap two elements in a list.

Q84. Write a Python program to find N largest element from a list.

Q85. Write a Python program to find cumulative sum of a list.

Q86. Write a Python program to check if a string is palindrome or not.

Q87. Write a Python program to remove i'th element from a string.

Q88. Write a Python program to check if a substring is present in a given string.

Q89. Write a Python program to find words which are greater than given length k.

Q90. Write a Python program to extract unquire dictionary values.

Q91. Write a Python program to merge two dictionary.

Q92. Write a Python program to convert a list of tuples into dictionary.
```
Input : [('Sachin', 10), ('MSD', 7), ('Kohli', 18), ('Rohit', 45)]
Output : {'Sachin': 10, 'MSD': 7, 'Kohli': 18, 'Rohit': 45}
```

Q93. Write a Python program to create a list of tuples from given list having number and its cube in each tuple.
```
Input: list = [9, 5, 6]
Output: [(9, 729), (5, 125), (6, 216)]
```

Q94. Write a Python program to get all combinations of 2 tuples.
```
Input : test_tuple1 = (7, 2), test_tuple2 = (7, 8)
Output : [(7, 7), (7, 8), (2, 7), (2, 8), (7, 7), (7, 2), (8, 7), (8, 2)]
```

Q95. Write a Python program to sort a list of tuples by second item.
```
Input : [('for', 24), ('Geeks', 8), ('Geeks', 30)] 
Output : [('Geeks', 8), ('for', 24), ('Geeks', 30)]
```

Q96. Write a python program to print below pattern.
```
* 
* * 
* * * 
* * * * 
* * * * * 
```
```
# Print pyramid pattern using For loop.
rows = 5
for i in range(rows):
    for j in range(i+1):
        print("* ", end="")
    print("\n")
```
Q97. Write a python program to print below pattern.
```
    *
   **
  ***
 ****
*****
```
```
# Print pyramid pattern using while loop.
n=5;i=0
while(i<=n):
  print(" " * (n - i) +"*" * i)
  i+=1
  ```

Q98. Write a python program to print below pattern.
```
    * 
   * * 
  * * * 
 * * * * 
* * * * * 
```
```
# Function to demonstrate printing pattern triangle
def triangle(n):
	
	# number of spaces
	k = n - 1

	# outer loop to handle number of rows
	for i in range(0, n):
	
		# inner loop to handle number spaces
		# values changing acc. to requirement
		for j in range(0, k):
			print(end=" ")
	
		# decrementing k after each loop
		k = k - 1
	
		# inner loop to handle number of columns
		# values changing acc. to outer loop
		for j in range(0, i+1):
		
			# printing stars
			print("* ", end="")
	
		# ending line after each row
		print("\r")

# Driver Code
n = 5
triangle(n)
```

Q99. Write a python program to print below pattern.
```
1 
1 2 
1 2 3 
1 2 3 4 
1 2 3 4 5
```
```
# Function to demonstrate printing pattern of numbers
def numpat(n):
	
	# initialising starting number
	num = 1

	# outer loop to handle number of rows
	for i in range(0, n):
	
		# re assigning num
		num = 1
	
		# inner loop to handle number of columns
			# values changing acc. to outer loop
		for j in range(0, i+1):
		
				# printing number
			print(num, end=" ")
		
			# incrementing number at each column
			num = num + 1
	
		# ending line after each row
		print("\r")

# Driver code
n = 5
numpat(n)
```

Q100. Write a python program to print below pattern.
```
A 
B B 
C C C 
D D D D 
E E E E E 
```
```
# Function to demonstrate printing pattern of alphabets
def alphapat(n):
	
	# initializing value corresponding to 'A'
	# ASCII value
	num = 65

	# outer loop to handle number of rows
	# 5 in this case
	for i in range(0, n):
	
		# inner loop to handle number of columns
		# values changing acc. to outer loop
		for j in range(0, i+1):
		
			# explicitly converting to char
			ch = chr(num)
		
			# printing char value
			print(ch, end=" ")
	
		# incrementing number
		num = num + 1
	
		# ending line after each row
		print("\r")

# Driver Code
n = 5
alphapat(n)
```


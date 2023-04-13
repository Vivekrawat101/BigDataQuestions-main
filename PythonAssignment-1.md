## Assignment Part-1
Q1. Why do we call Python as a general purpose and high-level programming language?

Answer: Python is called a general purpose and high-level programming language because it is used to 
develop huge variety of software application in multiple domains, it can run on all platforms, has library support, easy to access, understand and easy to use.

Q2. Why is Python called a dynamically typed language?

Answer: It is a dynamically typed language because we don't need to assign a datatype to a variable definition, datatype is smartly identified by the compiler during runtime. 

Q3. List some pros and cons of Python programming language?

Answer: 
PROS: Beginner-friendly
      Extensive Libraries
      Highly Scalable
      Portable
      Flexible and Extensible

CONS: Issues with design
      Slower than compiled languages
      High memory consumption
      Garbage collection leads to potential memory losses
      Complex multithreading

Q4. In what all domains can we use Python?

Answer: Big Data
        Data Science
        Application Development 
        AI & Machine Learning
        Automation 
        Audio/Video Applications
        Console Applications
        Desktop GUI

Q5. What are variable and how can we declare them?

Answer:A Variable is nothing but a programming element used to define, store, and perform operations on the input data. Python variables are of four different types: Integer, Long Integer, Float, and String.

We can define variables as follows:
pen = 'Parker' # String variable 
num = 8 # Int variable
dec = 8.01 # float variable
lint = int("111111111111111111111")  # long int variable

Q6. How can we take an input from the user in Python?

Answer: We use input() function to take input values from the user.

Q7. What is the default datatype of the value that has been taken as an input using input() function?

Answer : Default datatype of user input value is String.

Q8. What is type casting?

Answer : To convert datatype of a variable to a different datatype.

Q9. Can we take more than one input from the user using single input() function? If yes, how? If no, why?

Answer: YES!
If all the inputs are in single line then we can use : input().split()


Q10. What are keywords?
Answer: Python keywords are special reserved words that have specific meanings and purposes and can't be used for anything but those specific purposes.
example : in = 10  
          or = 1
          for = 1
          all will generate compile time error

Q11. Can we use keywords as a variable? Support your answer with reason.

Answer: No, we can't use keywords as variable because keywords are reserved words for compiler and has specific meaning attached to them.

Q12. What is indentation? What's the use of indentaion in Python?

Answer: Indentation refers to the spaces at the beginning of a code line.Python uses indentation to indicate a block of code. By default, a Python indentation is equal to 4 whitespaces.

Q13. How can we throw some output in Python?

Answer: We use print() function to display an output. For example:
print("Hello World") #prints Hello World
color = 'blue'
print(f'color is : {color}') #prints color is : blue

Q14. What are operators in Python?

Answer:Special symbols that designate that some sort of computation should be performed.

Q15. What is difference between / and // operators?

Answer: In Python programming, you can perform division in two ways. The first one is Float Division("/") and the second is Integer Division("//") or Floor Division.
5/2 = 2.5
5//2 = 2

Q16. Write a code that gives following as an output.
```
iNeuroniNeuroniNeuroniNeuron
```
Answer: 
companyName ="iNeuron"
print(f'{companyName}{companyName}{companyName}{companyName}')

Q17. Write a code to take a number as an input from the user and check if the number is odd or even.

num = int(input())
if num % 2 == 0 : 
    print(f'{num} is even')
else:
    print(f'{num} is odd')

Q18. What are boolean operator?

Answer: Boolean Operators are simple words (AND, OR, NOT or AND NOT) used as conjunctions to combine or exclude keywords in a search,

Q19. What will the output of the following?
```
1 or 0

0 and 0

True and False and True

1 or 0 or 0
```
Answer: 

1 or 0 -> 1

0 and 0 -> 0

True and False and True -> False

1 or 0 or 0 -> 1

Q20. What are conditional statements in Python?

Answer: Conditional statements are used to handle conditions in python program. These statements guide the program while making decisions based on the conditions encountered by the program.

Python has 3 key Conditional Statements that you should know:

if statement
if-else statement
if-elif-else ladder

Q21. What is use of 'if', 'elif' and 'else' keywords?

Answer: 
if -> The if statement is a conditional statement in python, that is used to determine whether a block of code will be executed or not. Meaning if the program finds the condition defined in the if statement to be true, it will go ahead and execute the code block inside the if statement.

else-> else statement works in conjuncture with the if statement to execute a code block when the defined if condition is false.

elif->The elif statement is used to check for multiple conditions and execute the code block within if any of the conditions evaluate to be true.The elif statement is similar to the else statement in the context that it is optional but unlike the else statement, there can be multiple elif statements in a code block following an if statement.

Q22. Write a code to take the age of person as an input and if age >= 18 display "I can vote". If age is < 18 display "I can't vote".
Answer:
age = int(input("ENTER YOUR AGE : "))
print("I can vote") if age >= 18 else print("I can't vote")

Q23. Write a code that displays the sum of all the even numbers from the given list.
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```
Answer:
numbers = [12, 75, 150, 180, 145, 525, 50]
sum = 0
for n in numbers:
    if n%2==0:
        sum+=n
print(sum)

Q24. Write a code to take 3 numbers as an input from the user and display the greatest no as output.

Answer:

#if inputs are in single line space separated
numbers = list(map(int, input().split()))   
max = 0
for n in numbers:
    if n>max:
        max=n
print(max)

Q25. Write a program to display only those numbers from a list that satisfy the following conditions

- The number must be divisible by five

- If the number is greater than 150, then skip it and move to the next number

- If the number is greater than 500, then stop the loop
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```
Answer:

numbers = [12, 75, 150, 180, 145, 525, 50]

for n in numbers:
    
    if n>500:
        break
    else:
        if n>150:
            continue 
        if n%5==0:
            print(n)

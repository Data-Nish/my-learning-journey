# my-learning-journey
Python Core Fundamentals
# Python History
Python was created by Guido Van Rossum born in 1956. Started programming project as a hobby in December 1989. He is a big fan of 'Monty Python's Flying Circus', sitcom series, so chose Python as a working title for the project. In 1999, he defined four goals for Python 
1. An EASY and INTUITIVE LANGUAGE as powerful as major competitors
2. OPEN SOURCE, so anyone can contribute to it's development
3. Code is UNDERSTANDABLE in plain English
4. Suitable for everyday tasks
   
Python still occupies a high rank in the top ten of the PYPL PopularitY of Programming Language.

# What is Python?
Python is a tool, not a reptile. Python is a widely-used, interpreted, object-oriented, and high-level programming language with dynamic semantics (set of rules determing the program makes sense) used for general purpose programming.

# What makes Python Special? 
Easy to learn
Easy to teach
Easy to use
Easy to understand
Easy to obtain, install and deploy (https://www.python.org/downloads/)

Interesting fact - Python Software Foundation (PSF), a community that aims to develop, improve, expand, abd popularize Python and it's environment

# Drawbacks
1. It's not a speed demon - doesn't deliver exceptional performance
2. Debugging Python Code can be more difficult than other languages

# Python Variables
Variables are used to store and retrieve data from the memory. We can store value in a variable by either ASSIGNING a value to a variables or GETTING the value as INPUT from user.
A variable should start with a letter or an underscore and cannot start with numbers.

= is an Assignment Operator e.g. a=b assigns a with thw value of b

1. Assigning Values - Two ways of assigning values to a variable:
   
   a. Assigning a Single Value
   name = 'Jen'

   salary = 20000

   print(name)

   print(salary)

   b. Multiple Assignment : Assigning multiple values:

   a=b=c=10
   
   x,y,z=10,20,30
   
   print(y)
   
   print(z)
   
   print(a)
   
   20
   
   30
   
   10

2. Getting User Input - To get input from user in python and then assign that value to a python variable, we need to user the 'INPUT' function.
To use the input function we also need to show a 'Prompt' to user to asking them to enter a value.

name = input("Enter your name: ")

# Python DataTypes
A Data Type indicates to the interpreter what type of data is stored in a variable e.g. Number, Text, etc
1. Integer - numerical type without fractional component
2. Float - another numerical type with fractional component
3. String - Character data type within quotes. To encode an apostrophe inside a string you can use either escape character('\'). e.g. 'I\'m happy.' or use double quotes e.g. "I'm happy." 
4. Boolean - are two constant objects True and False used to represent truth values (in numeric contexts 1 is True, while 0 is False.)

# Conditional Statements
It is the 'decision-making' center of code. These statement allows the program to act depending on whether a specific condition is true or false. In real life, this is how we think: 'If it is raining, I will take an umbrella. If it is not raining, I will wear sunglasses.'

Fortunately, computers know only two kinds of answers: 

a. yes, this is true
b. no, this is false

Python uses a set of very special operators
Priority	   Operator	
1         	+, -	         unary

2	         **	

3	         *, /, //, %	

4	         +, -	         binary

5	         <, <=, >, >=	

6	         ==, !=

Three types of Conditional Statements

1. If

2. If-else
 
3. If-elif
   


If syntax
---------
if true_or_not:

   do_this_if_true

the 'if' keyword
an expression (a question or an answer) whose value will be interpreted solely in terms of True (when its value is non-zero) and False (when it is equal to zero);
a colon followed by a newline
an indented instruction or set of instructions (at least one instruction is absolutely required), it's important to make all indentations exactly the same

How does that statement work?

If the true_or_not expression represents the truth (i.e., its value is not equal to zero), the indented statement(s) will be executed;
if the true_or_not expression does not represent the truth (i.e., its value is equal to zero), the indented statement(s) will be omitted (ignored), and the next executed instruction will be the one after the original indentation level.

if the_weather_is_good:

    go_for_a_walk()

have_lunch()

having lunch is not a conditional activity and doesn't depend on the weather

CONDITIONALLY EXECUTED STATEMENTS HAVE TO BE INDENTED

2. if-else statement
   Syntax
   ------
if true_or_false_condition:

    perform_if_condition_true

else:

    perform_if_condition_false

the 'else' keyword says what to do if the condition specified for the if is not met (note the colon after the word).

The if-else execution goes as follows:

if the condition evaluates to True (its value is not equal to zero), the perform_if_condition_true statement is executed, and the conditional statement comes to an end;
if the condition evaluates to False (it is equal to zero), the perform_if_condition_false statement is executed, and the conditional statement comes to an end.

if the_weather_is_good:

    go_for_a_walk()

else:

    go_to_a_theater()
have_lunch()

If the weather is good, we'll go for a walk. Otherwise, we'll go to a theatre. No matter if the weather is good or bad, we'll have lunch afterwards (after the walk or after going to the theatre).

Nested if-else Statements
instruction placed after the if is another if

if the_weather_is_good:

    if nice_restaurant_is_found:

        have_lunch()
    
    else:
    
        eat_a_sandwich()

else:

    if tickets_are_available:
       
        go_to_the_theater()
    
    else:
    
        go_shopping()

Here are two important points:
this use of the if statement is known as nesting;remember that every else refers to the if which lies at the same indentation level; determine how the ifs and elses pair up;

indentation improves readability, 

3. elif Statement
   -------------- 
 it's a shorter form of else if. The elif keyword used when we have multiple conditions and want to check them one by one.

if the_weather_is_good:

    go_for_a_walk()

elif tickets_are_available:

    go_to_the_theater()

elif table_is_available:

    go_for_lunch()

else:

    play_chess_at_home()

If the weather is fine, we'll go for a walk, otherwise if we get tickets, we'll go to the theater, otherwise if there are free tables at the restaurant, we'll go for lunch; if all else fails, we'll return home and play chess. The way to assemble subsequent if-elif-else statements is sometimes called a 'cascade'.

It mustn't use else without a preceding if;

else is always the last branch of the cascade, regardless of whether you've used elif or not;

else is an optional part of the cascade, and may be omitted;

if there is an else branch in the cascade, only one of all the branches is executed;

if there is no else branch, it's possible that none of the available branches is executed.

# LOOPS

Performing a certain part of the code more than once is called a loop. Looping is the process in which we have a some code that gets executed repeatedly until a particular condition is satisfied.
There are two kinds of loops used in python - 

01. For
 - The for statement is used to loop over a group or collection of data. Sometimes it's more important 'to count the "turns" of the loop' than to check the conditions
   -----
  the for loop is designed to do more complicated tasks - it can "browse" large collections of data item by item 

syntax
-----
for i in range(100):
    # do_something()
    pass

the for keyword opens the for loop; note - there's no condition after it; you don't have to think about conditions, as they're checked internally, without any intervention

any variable after the for keyword is the 'control variable' of the loop (which is 'i' in the syntax above); it counts the loop's turns, and does it automatically

the 'in' keyword introduces a syntax element describing the range of possible values being assigned to the control variable

the 'range()' function (this is a very special function) is responsible for generating all the desired values of the control variable

note the 'pass' keyword inside the loop body - it does nothing at all; it's an 'empty instruction' - we put it here because the for loop's syntax demands 'at least one instruction inside the body' (by the way - if, elif, else and while express the same thing)

# Example 1
for num in range(0,10):
   print('The value of num is', num)

   ans
   ---
   0 to 9
   
   the loop has been executed ten times (it's the range() function's argument)
   # The range() function may also accept three arguments -  'starting number' of the sequence , second argument tells the function 'where to stop' the sequence and  the third argument indicates the 'step' -  increment (the default value of the increment is 1)

   # Example 2
   for i in range(2, 8, 3):
       print("The value of i is currently", i)

 # output
The value of i is currently 2
The value of i is currently 5
   
   the last control variable's value is 9 (not 10, as it starts from 0, not from 1) in example 1

02. While
- The while statement simply loops until a condition is evaluates to False
   ------
   syntax
   ------
   while conditional_expression:
       instruction

  If you notice some similarities to the 'if' instruction, the syntactic difference is only one: you use the word 'while' instead of the word if. The semantic difference is more important: when the condition is met, 'if' performs its statements _only once_; 'while' repeats the execution as long as the condition evaluates to True.
------------------------------------------------------------------------------------
count = 0
while count <10:
   print(count)
   count=+1

Note: all the rules regarding indentation are applicable here, too

syntax 
------
while conditional_expression:
    instruction_one
    instruction_two
    instruction_three
    :
    :
    instruction_n
    
if you want to execute more than one statement inside one while, you must (as with if) indent all the instructions in the same way;

an instruction or set of instructions executed inside the while loop is called the 'loop's body';

if the condition is False (equal to zero) as early as when it is tested for the first time, the body is not executed even once

the body 'should be able to change the condition's value', because if the condition is True at the beginning, the body might run continuously to infinity 

An infinite loop
----------------
An infinite loop, also called an endless loop, is a sequence of instructions in a program which repeat indefinitely (loop endlessly.)

while True:
    print("I'm stuck inside a loop.")

This loop will infinitely print "I'm stuck inside a loop." on the screen.

 To terminate your program, just press Ctrl-C (or Ctrl-Break on some computers)
 ---------------------------------------------


Using a 'counter' variable to exit a loop
----------------------------------------

counter = 5
while counter:
    print("Inside the loop.", counter)
    counter -= 1
print("Outside the loop.", counter)

or
--

counter = 5
while counter != 0:
    print("Inside the loop.", counter)
    counter -= 1
print("Outside the loop.", counter)

Both generate the same output, anyone can be used. First one is preferred mostly
output
------
Inside the loop. 5
Inside the loop. 4
Inside the loop. 3
Inside the loop. 2
Inside the loop. 1
Outside the loop. 0


# Example 2 While loop

odd_numbers = 0
even_numbers = 0

# Read the first number.
number = int(input("Enter a number or type 0 to stop: "))

# 0 terminates execution.
while number != 0:
    # Check if the number is odd.  
    if number % 2 == 1:  # if a number divided by 2 leaves a remainder of 1 (odd) or 0 (even)
        # Increase the odd_numbers counter.
        odd_numbers += 1
    else:
        # Increase the even_numbers counter.
        even_numbers += 1
    # Read the next number.
    number = int(input("Enter a number or type 0 to stop: "))

# Print results.
print("Odd numbers count:", odd_numbers)
print("Even numbers count:", even_numbers)

 note that these two forms are equivalent:
------------------------------------------
while number != 0: and while number:

or
--

if number % 2 == 1: and if number % 2:


# Data Structures
List
----
These indexes start from zero and are assigned in an increasing order i.e. from zero to n – 1 where n is number of items in that lists. These lists can store data of multiple data types, e.g. Integer, String, Float, etc. 
Step 1: To creatw

Tuple

Dictionary

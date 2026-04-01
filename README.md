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

01. For - The for statement is used to loop over a group or collection of data
for num in range(0,10):
print(num)

2. While - The while statement simply loops until a condition is evaluates to False
count = 0
while count <10:
   print(count)
   count=+1

# Data Structures
List

Tuple

Dictionary

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

= is an Assignment Operator e.g. a=b assigns a with the value of b

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

 Priority   	Operator	
------------------------------------------
1	            ~, +, -	            unary

2	            **	

3	            *, /, //, %	

4	            +, -	               binary

5	            <<, >>	  

6	            <, <=, >, >=	

7	            ==, !=	

8	            &	

9	            |	   

10	            =, +=, -=, *=, /=, %=, &=, ^=, |=, >>=, <<=

Note
----
Think of Bitwise Shifting as moving digits left or right
1. The Decimal Comparison (The "Power of 10" trick)
In our normal math (Base 10):

If you take 5 and shift it left (add a zero), it becomes 50. You just multiplied by 10.

If you take 50 and shift it right (remove a digit), it becomes 5. You just divided by 10.

2. The Binary Reality (The "Power of 2" trick)

Computers use Base 2. So, instead of 10, everything happens in twos.

Left Shift (<<): Moving bits to the left is like doubling the number.17 << 1 is $17 \times 2 = 34$17 << 2 is $17 \times 4 = 68$ (Doubled twice)

Right Shift (>>): Moving bits to the right is like cutting the number in half.17 >> 1 is $17 // 2 = 8$ (The ".5" is chopped off) # right-shifting is the same as floor division (//); you lose the remainder.

Digraphs: Just a fancy word for a symbol made of two characters (<< or >>). High Priority: In a long math equation, Python will perform the "shifts" before it performs basic addition or subtraction.
--------

#Example
--------
var = 17

var_right = var >> 1  #17//2=8

var_left = var << 2   #17*4=68

print(var, var_left, var_right)

output
------
17 68 8

# Three types of Conditional Statements

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

# CONDITIONALLY EXECUTED STATEMENTS HAVE TO BE INDENTED

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

indentation improves readability.

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

   ans/Output
   ---
The value of num is 0
The value of num is 1
The value of num is 2
The value of num is 3
The value of num is 4
The value of num is 5
The value of num is 6
The value of num is 7
The value of num is 8
The value of num is 9
   
   the last control variable's value is 9 (not 10, as it starts from 0, not from 1) in example 1
   the loop has been executed ten times (it's the range() function's argument)
   # The range() function may also accept three arguments -  'starting number' of the sequence , second argument tells the function 'where to stop' the sequence and  the third argument indicates the 'step' -  increment (the default value of the increment is 1)

   # Example 2
   for i in range(2, 8, 3):
   
       print("The value of i is currently", i)

 # output
The value of i is currently 2
The value of i is currently 5
   
Note: if the set generated by the range() function is empty, the loop won't execute its body at all.
----
Just like here - there will be 'no output' below
# empty range() function example = empty output
for i in range(1, 1):

    print("The value of i is currently", i)

# range has to be sorted in ascending order. This means that the range()'s second argument must be  greater than the first. there will be 'no output' for this one as well

for i in range(2, 1):

    print("The value of i is currently", i)

# Example 
power = 1

for expo in range(16):

    print("2 to the power of", expo, "is", power)
    
    power *= 2

# output

2 to the power of 0 is 1
2 to the power of 1 is 2
2 to the power of 2 is 4
2 to the power of 3 is 8
2 to the power of 4 is 16
2 to the power of 5 is 32
2 to the power of 6 is 64
2 to the power of 7 is 128
2 to the power of 8 is 256
2 to the power of 9 is 512
2 to the power of 10 is 1024
2 to the power of 11 is 2048
2 to the power of 12 is 4096
2 to the power of 13 is 8192
2 to the power of 14 is 16384
2 to the power of 15 is 32768

# Explanation
This is a very efficient way to generate a mathematical sequence. By using power *= 2 at the end of each loop, the program ensures that the power variable is always ready for the next iteration's print statement.

Note that the loop runs 16 times, but because it starts at 0, the highest exponent shown is 15.

   *************************************************************************************************

02. While
- The while statement simply loops until a condition is evaluates to False
   ------
   syntax
   ------
   while conditional_expression:
  
       instruction

  If you notice some similarities to the 'if' instruction, the syntactic difference is only one: you use the word 'while' instead of the word if. The semantic difference is more important: when the condition is met, 'if' performs its statements _only once_; 'while' repeats the execution as long as the condition evaluates to True.
------------------------------------------------------------------------------------

# This code will result in an infinite loop, The reason is a tiny but very important typo in the last line: count=+1
count = 0
while count <10:
   print(count)
   count=+1  #count = +1 simply 'assigns' the value positive 1 to the variable.

Explanation
-----------

The loop starts at 0; It prints 0; It sets count to 1; It checks the condition : is 1<0? Yes; It prints 1; It sets count to 1 again ; It checks te condition : Is 1<10? Yes. 'Since 1 is  always less than 10, the loop never finds a reason to stop.'

In Python, =+ is not the same as +=
-----------------------------------
count += 1 adds 1 to the current value (incrementing)

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


# break and continue statements
--------------------------------

Normally, a loop is like a train track—it has to go through every station (line of code) before it can start the next lap. These two statements let you break that rule. Think of break and continue as "emergency exits" or "shortcuts" inside a loop.

1. break (The Stop or Exit Button)
---------
Stops the loop entirely. The program jumps immediately to the first line of code after the loop.
Kills the loop. The loop ends immediately.

# break - example

print("The break instruction:")
for i in range(1, 6):
    if i == 3:
        break
    print("Inside the loop.", i)
print("Outside the loop.")

# Output
The break instruction:
Inside the loop. 1
Inside the loop. 2
Outside the loop.


2. continue (the Skip Button)
------------
Skips the rest of the current lap and jump straight to the start of the next one.
Skips the curret turn. The loop restarts at the next turn.

You could achieve the same thing using complex if statements. However, Python includes them because they make your code cleaner, shorter, and easier to read.

# continue - example

print("\nThe continue instruction:")
for i in range(1, 6):
    if i == 3:
        continue
    print("Inside the loop.", i)
print("Outside the loop.")

# Output
The continue instruction:
Inside the loop. 1
Inside the loop. 2
Inside the loop. 4
Inside the loop. 5
Outside the loop.



# Data Structures
List
----
These indexes start from zero and are assigned in an increasing order i.e. from zero to n – 1 where n is number of items in that lists. These lists can store data of multiple data types, e.g. Integer, String, Float, etc. 

To create List
---------------
Use the list function or use empty brackets
name=list()
print(name)

age=[]
print(age)

# Output
[]
[]

Initialize
------------------
You can initialize a list with some data while creating the list, by passing values inside the list function or brackets

age =[25, 33, 19]
print (age)

# output 
[25, 33, 19]
0   1   2 - this is index (the value inside the brackets which selects one element of the list is called an index)

Append
------
You can add data to the end of list by calling the append method on the lists

age.append(40)
print (age)

# Output
[25, 33, 19, 40]

Delete (pop or del)
-------------------
You can delete an element in a list by calling the pop method on it. Pop will delete the element at the end of the list

age.pop()
print(age)

# Output
[25, 33, 19]

You can also delete an element at a particular index, by passing the index in as parameters in the function call

age.pop(0)
print(age)

# output
[33, 19]
# Another Example using 'del'

numbers = [10, 5, 7, 2, 1]
print("Original list content:", numbers)  # Printing original list content.

numbers[0] = 111
print("\nPrevious list content:", numbers)  # Printing previous list content.

numbers[1] = numbers[4]  # Copying value of the fifth element to the second.
print("Previous list content:", numbers)  # Printing previous list content.

print("\nList's length:", len(numbers))  # Printing previous list length.

###

del numbers[1]  # Removing the second element from the list.
print("New list's length:", len(numbers))  # Printing new list length.
print("\nNew list content:", numbers)  # Printing current list content.

# Output

Original list content: [10, 5, 7, 2, 1]

Previous list content: [111, 5, 7, 2, 1]
Previous list content: [111, 1, 7, 2, 1]

List's length: 5
New list's length: 4

New list content: [111, 7, 2, 1]


Before we start talking about tuples and dictionaries, we have to introduce two important concepts: 
# sequence types and mutability

A sequence type is a type of data in Python which is able to store more than one value (or less than one, as a sequence may be empty), and these values can be sequentially (hence the name) browsed, element by element.
As the 'for' loop is a tool especially designed to iterate through sequences, we can express  a sequence is data which can be scanned by the for loop.

The second notion - mutability - is a property of any of Python's data that describes its readiness to be freely changed during program execution. There are two kinds of Python data: mutable and immutable.

# Mutable data can be freely updated at any time
Immutable data cannot be modified

# Tuples - A tuple is an immutable sequence type. Tuples prefer to use parenthesis
Tuples are also used to store collection of in a sequential order, the difference is that it is immutable. Immutable means that once you create a tuple, you cant make changes to it, i.e. add items, remove items, swap items.

Like lists, elements in tuples are also accessed using their indexes. Tuples can also store data of multiple types such as Integer, float, boolean, etc. 

Create
-------
To create  a tuple with some values you can either use the tuple function or use the comma syntax

# example of empty tuples
Options = ()
names = tuple()
print(Options)
print(names)

# Output
()
()

# example of one-element tuple
one_element_typle_1 = (1, )
print(one_element_typle_1)
one_element_typle_2 = (1., )
print(one_element_typle_2)

# Output
(1,)
(1.0,)

Initialize
----------
To use the comma syntax you need to have a few values separated by commas and assign them to a variable

# Example
age =25,18,21
print(age)

# Output
(25, 18, 21)

0     1   2  # indexes of above tuple elements

Search
------
To check if a particular element exists in the tuple we use the membership operator (using the ‘in’ keyword), which returns True if element exists and False if it does not

# Example
21 in age

# Output
True

You can also use the index method to find the 'index of a particular element' in a tuple. It returns the index if the element is found if not then throws an error.

# Example
age.index(21)

# Output
2

# Example
my_tuple = (1, 10, 100)

t1 = my_tuple + (1000, 10000)
t2 = my_tuple * 3  #3 times my_tuple

print(len(t2))
print(t1)
print(t2)
print(10 in my_tuple)
print(-10 not in my_tuple)

# Output
9
(1, 10, 100, 1000, 10000)
(1, 10, 100, 1, 10, 100, 1, 10, 100)
True
True

# interesting fact about tuple
One of the most useful tuple properties is their ability to appear on the left side of the assignment operator. It is an elegant tool to swap two variables' values. A tuple's elements can be variables

Let's see an example
--------------------
var = 123

t1 = (1, )
t2 = (2, )
t3 = (3, var)

t1, t2, t3 = t2, t3, t1

print(t1, t2, t3)

# output

(2,) (3, 123) (1,)

It shows three tuples interacting - in effect, the values stored in them "circulate" - t1 becomes t2, t2 becomes t3, and t3 becomes t1

Slice
-----
Slicing is a powerful way to extract a specific portion (a "slice") of a sequence, such as a string, list, or tuple.
To slice a list we need to provide the index from where you wish to start the slice and index before which the slice ends like age[1:4]

# Example
age =25,18,21, 33, 35
print(age[1:4])

# output
(18, 21, 33)
********************************************************************************************************

Dictionary - a dictionary is a set of key-value pairs. The list of pairs is surrounded by 'curly braces', while the pairs themselves are separated by 'commas', and the keys and values by 'colons'.
----------
It's not a sequence type (but can be easily adapted to sequence processing) and it is mutable. The Python dictionary works in the same way as a bilingual dictionary.

Note:
-----
Each key must be unique - it's not possible to have more than one key of the same value;

a key may be any immutable type of object: it can be a number (integer or float), or even a string, but not a list;

a dictionary is not a list - a list contains a set of numbered values, while a dictionary holds pairs of values;

the len() function works for dictionaries, too - it returns the numbers of key-value elements in the dictionary;

a dictionary is a one-way tool - if you have an English-French dictionary, you can look for French equivalents of English terms, but not vice versa.

# Example
dictionary = {"cat": "chat", "dog": "chien", "horse": "cheval"}
phone_numbers = {'boss': 5551234567, 'Suzy': 22657854310}
empty_dictionary = {}

print(dictionary)
print(phone_numbers)
print(empty_dictionary)

# Output
{'cat': 'chat', 'dog': 'chien', 'horse': 'cheval'}
{'boss': 5551234567, 'Suzy': 22657854310}
{}

Create
------
To create an empty dictionary you can either use the dict function or use the curly braces syntax

# Example
names = {}
age = dict()
print(age)
print(names)

# Output
{}
{}

Initialize
----------
To initialize a dictionary with some values you can either pass some nested data structures to dict function or use the curly braces syntax

# Example
age_list = [['a',1], ['b',2], ['c',3]]

age = dict(age_list)

print(age)

# Output
{'a': 1, 'b': 2, 'c': 3}

Add
---
To add a new key value pair by using this syntax:

dict_name[key] = value

# Example
age['d'] = 5

print(age)

# Output
{'a': 1, 'b': 2, 'c': 3, 'd': 5}

Remove
------
To remove an element just use the 'del' keyword with the key dictionary name e.g. del age[‘d’]

# Example
del age['d']

print(age)

# Output
{'a': 1, 'b': 2, 'c': 3}

Search
------
To search a value you need to use the membership operator with the key, If the key is found it returns true else it returns false

# Example
'a' in age

# Output
True

NOTE:
-----

(*) In Python 3.6x dictionaries have become ordered collections by default. Your results may vary depending on what Python version you're using.

***************************************************************************************************

# Creating a Function - A function is a block of code that performs a specific task when the function is called (invoked). You can use functions to make your code reusable, better organized, and more readable. Functions can have parameters and return values.

This is what the simplest function definition looks like:

syntax
------
def function_name():

    function_body


It always starts with the keyword 'def' (for define)

next after def goes the 'name of the function' (the rules for naming functions are exactly the same as for naming variables)

after the function name, there's a place for a 'pair of parentheses (they contain nothing here, but that will change soon)

the line has to be ended with a 'colon'

the line directly after def begins the 'function body' ‒ a couple (at least one) of necessarily 'nested instructions', which will be executed every time the function is invoked; note: the 'function ends where the nesting ends', so you have to be careful.

Another Syntax
--------------
def add_two_numbers(x,y):

   print ("adding two number")

   return x+ y

   add_two_numbers = 'Name' of the Function
   (x,y) = 'Parameters' or Function Arguments
   x+y = 'return' statement

Meanings
--------
The name of the function is like a naming a variable and follows the same rules

Parameters or Function Arguments are the variables or data that we want our function to work on,e.g., numbers to be added
Note:
-----
You can have any number of parameters be accepted in your function or no parameters if your function does not need it

Return - You can have no return value at the end by simply omitting the return statement in case you so not wish your function to return a value

# Types of Functions 

There are at least 'four' basic types of functions in Python:

'built-in functions' which are an integral part of Python (such as the print() function). You can see a complete list of Python built-in functions at https://docs.python.org/3/library/functions.html 

the ones that come from 'pre-installed modules' 

'user-defined functions' which are written by users for users - you can write your own functions and use them freely in your code

the 'lambda functions'


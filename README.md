# Python3 Workshop

Topics we will be covering in this worlshop:
- [Python3 Workshop](#python3-workshop)
  - [What is Python?](#what-is-python)
  - [Comments in Python](#comments-in-python)
  - [Basic Data Structures](#basic-data-structures)
    - [Numbers](#numbers)
      - [Types of numbers](#types-of-numbers)
      - [Basic Arithmetic](#basic-arithmetic)
      - [Variable Assignment](#variable-assignment)
      - [Rules for naming variables](#rules-for-naming-variables)
      - [Dynamic Typing](#dynamic-typing)
      - [Determining type of variable](#determining-type-of-variable)
  - [Strings](#strings)
    - [Indexing and Slicing in Strings](#indexing-and-slicing-in-strings)
    - [String Properties](#string-properties)
    - [String Methods](#string-methods)
    - [String Formatting](#string-formatting)
  - [List](#list)
    - [Indexing and Slicing in List](#indexing-and-slicing-in-list)
    - [List Methods](#list-methods)
    - [Nested List](#nested-list)
    - [List Comprehension](#list-comprehension)
  - [Dictonary](#dictonary)
    - [Dictonary Methods](#dictonary-methods)
    - [Tuples](#tuples)
    - [Tuple Methods](#tuple-methods)
    - [Tuples are Immutable!](#tuples-are-immutable)
    - [Use of Tuple](#use-of-tuple)
  - [Sets](#sets)
  - [Booleans](#booleans)
  - [File Handling](#file-handling)
    - [Writing to a File](#writing-to-a-file)
- [Python Statements](#python-statements)
  - [if, elif, else Statements](#if-elif-else-statements)
- [Loops](#loops)
  - [For Loop](#for-loop)
  - [While Loop](#while-loop)
    - [Range](#range)
    - [Enumerate](#enumerate)
    - [Zip](#zip)
    - [In](#in)
    - [Random](#random)
  - [Functions](#functions)
  - [Args and Kwargs](#args-and-kwargs)
  - [Lambda Expressions, Map, and Filter](#lambda-expressions-map-and-filter)
    - [Map Function](#map-function)
    - [Filter Function](#filter-function)
    - [Lambda expression](#lambda-expression)
  - [Object Oriented Programming](#object-oriented-programming)
    - [Objects](#objects)
    - [Class](#class)
    - [Methods](#methods)
  - [Inheritance](#inheritance)
  - [Polymorphism](#polymorphism)
  - [Time to Practice](#time-to-practice)
  - [Some Resources to start your Python Journey](#some-resources-to-start-your-python-journey)
  - [References](#references)

## What is Python?

[![alt text](https://github.com/ishpreet-singh/python3-workshop/blob/master/assets/why-python.png)
](https://www.youtube.com/watch?v=Y8Tko2YC5hA)

![alt text](https://github.com/ishpreet-singh/python3-workshop/blob/master/assets/lets-begin.png)

## Comments in Python


    # This is a single line comment

    '''
        This is a multiline 
        comment.
    '''

## Basic Data Structures 

### Numbers

#### Types of numbers

Python has various "types" of numbers (numeric literals). We'll mainly focus on integers and floating point numbers.

Integers are just whole numbers, positive or negative. For example: 2 and -2 are examples of integers.

| Examples         | Number Type            |
|------------------|------------------------|
| 1, 2, 100, -100  | Integer                |
| 1.2,-0.5,2e2,3E2 | Floating Point Numbers |

#### Basic Arithmetic

```
# Addition
2 + 1
> 3
```

```
# Subtraction
2 - 1
> 1
```
```
# Multiplication
2 * 2
> 4
```
```
# Division
3 / 2
> 1.5
```
```
# Floor Division
7 // 4
> 1
```

```
# Modulo
7 % 4
> 3
```

```
# Powers
2 ** 3
> 8
```

```
# Can use parentheses to specify orders
(2+10) * (10+3)
> 156
```

#### Variable Assignment

```
# Let's create an object called "x" and assign it the number 5
x = 20
```

```
# Adding the objects
x + x
```

```
# Reassignment
x = 20
x = x + x
```

#### Rules for naming variables

1. Names can not start with a number.
2. There can be no spaces in the name, use _ instead.
3. Can't use any of these symbols :'",<>/?|\()!@#$%^&*~-+
4. It's considered best practice (PEP8) that names are lowercase.
5. Avoid using words that have special meaning in Python like "list" and "str"


#### Dynamic Typing

Python uses Dynamic Typing.

```
num = 2
num
> 2

num = "This is a number"
num
> This is a number
```

#### Determining type of variable

Python provides a build in function called `type` to check the type of variable.

```
x = 5
type(x)
> int

t = (4, 5)
type(t)
> tuple
```

Some common data types are:
* int (for integer)
* float
* str (for string)
* list
* tuple
* dict (for dictionary)
* set
* bool (for Boolean True/False)


## Strings

Strings in Python are actually a sequence, used to record textual info. 

```
# String using single quotes
'I am a string'

# String using double quotes
"I am also a string"
```

```
# Be careful with quotes!
' I'm using single quotes, but this will create an error'
```

Python provides a `print` method to print a string.
```
print('Hello, Welcome to the workshop')

print('This is an example how to use print method.\nI will be printed in next line because of \\n')
```

Python provides a `len` method to calculate the length of a string.

```
len('Python3 Workshop')
> 16
```

### Indexing and Slicing in Strings

```
# Assign s as a string
s = 'Hello World'

# Show first element (in this case a letter)
s[0]
> H

s[2]
> l
```

*We use : to perform Slicing*
```
# Grab everything past the first term all the way to the length of s which is len(s) However there's no change in s

s[1:]
> 'ello World'
```

```
# Grab everything UP TO the 3rd index

s[:3]
> 'Hel'
```

```
# What if we done provide any index in slicing?

s[:]
```

*Python also supports Negative Indexing*
```
# Last letter (one index behind 0 so it loops back around)

s[-1]
> 'd'

# Grab everything but the last letter

s[:-1]
> 'Hello Worl'
```

Step size in Slicing
```
# Grab everything, but go in step sizes of 2

s[::2]
> 'HloWrd'
```

Reverse a string

```
s[::-1]

> 'dlroW olleH'
```

### String Properties

*String are Immutable !*

```
# Let's try to change the first letter to 'x'
s[0] = 'x'
```

*Concate Strings*

```
s = s + ' conactenate me!!'
> Hello World concatenate me!
```

*String Multiplication*

```
label = 'p'
label * 5

> 'ppppp'
```

### String Methods

*Upper Case*

> Python has a build in method `upper` to get uppercase of a string.

```
# Upper Case a string
s.upper()

> 'HELLO WORLD CONCATENATE ME!'
```

Note these methods don't change the original string!
```
s.upper()
> 'HELLO WORLD CONCATENATE ME!'

s
> 'Hello World'
```

*Lower Case*
> Python has a build in method `lower` to get uppercase of a string.

```
s.lower()

> 'hello world concatenate me!'
```

*Split*

Extract words from string
```
# Split a string by blank space (this is the default)
s.split()

> ['Hello', 'World', 'concatenate', 'me!']


# Split by a specific element (doesn't include the element that was split on)
s.split('W')

> ['Hello ', 'orld concatenate me!']
```

### String Formatting


String formatting lets you inject items into a string rather than trying to chain items together.

```
player = 'Thomas'
points = 33


'Last night, '+player+' scored '+str(points)+' points.'  # concatenation

f'Last night, {player} scored {points} points.'          # string formatting
```

There are **three ways** to perform string formatting.

1. The oldest method involves placeholders using the modulo % character.
2. An improved technique uses the .format() string method.
3. The newest method, introduced with Python 3.6, uses formatted string literals, called f-strings.


*First Method* using **%**
```
print("I'm going to inject %s here." %'something')

> I'm going to inject something here.
```

```
x, y = 'some', 'more'
print("I'm going to inject %s text here, and %s text here."%(x,y))

> I'm going to inject some text here, and more text here.
```


*Second Method* using **.format()**
```
print('This is a string with an {}'.format('insert'))

> This is a string with an insert



print('The {2} {1} {0}'.format('fox','brown','quick'))

> The quick brown fox
```

*Third Method* using **f-strings**

```
name = 'Fred'

print(f"He said his name is {name}.")

> He said his name is Fred.
```

## List

List is an ordered sequence of elements.

```
# Assign a list to an variable named my_list
my_list = [1,2,3]
```

Unlike strings, they are **mutable**, meaning the elements inside a list can be changed!

```
my_list[1] = 5
my_list

> [1, 5, 3]
```

We just created a list of integers, but lists can actually hold different object types

```
my_list = ['A string',23,100.232,'o']
my_list 

> 'A string',23,100.232,'o'
```

Just like strings, list also has `len` to find length of string.
```
my_list = ['This', 'is', 'a', 'Python3', 'Workshop']
len(my_list)

> 5
```

### Indexing and Slicing in List

Indexing and slicing work just like in strings.

```
my_list = ['one','two','three',4,5]


# Grab element at index 0
my_list[0]

> 'one'


# Grab index 1 and everything past it
my_list[1:]
> ['two', 'three', 4, 5]

```


We can also use **+** to concatenate lists, just like we did for strings.
```
my_list + ['new item']

> ['one', 'two', 'three', 4, 5, 'new item']
```
**Note**: *This doesn't actually change the original list!*



We can also use the * for a duplication method similar to strings:
```
# Make the list double
my_list * 2

['one', 'two', 'three', 4, 5, 'one', 'two', 'three', 4, 5]
```

### List Methods

***append***
> Add an item to the end of the list

```
# Append
list1.append('append me!')
list1

> [1, 2, 3, 'append me!']
```

***pop***
> Remove the item at the given position in the list, and return it. If no index is specified, a.pop() removes and returns the last item in the list.

```
# Pop off the 0 indexed item
list1.pop(0)

> 1


list1

> [2, 3, 'append me!']

# Assign the popped element, remember default popped index is -1
popped_item = list1.pop()
```

***reverse***
> Reverse the elements of the list in place.

```
new_list = ['a','e','x','b','c']

# Use reverse to reverse order (this is permanent!)
new_list.reverse()

> ['c', 'b', 'x', 'e', 'a']
```

***sort***
> Sort the items of the list in place

```
# Use sort to sort the list (in this case alphabetical order, but for numbers it will go ascending)
new_list.sort()

new_list

> ['a', 'b', 'c', 'e', 'x']
```


### Nested List

```
# Let's make three lists
lst_1=[1,2,3]
lst_2=[4,5,6]
lst_3=[7,8,9]

# Make a list of lists to form a matrix
matrix = [lst_1,lst_2,lst_3]


matrix

> [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
```


```
# Grab first item in matrix object
matrix[0]

> [1, 2, 3]
```


```
# Grab first item of the first item in the matrix object
matrix[0][0]

> 1
```

### List Comprehension

```
nums = [1, 2, 3, 4]

squares = [ n * n for n in nums ]   

> [1, 4, 9, 16]
```


## Dictonary

Dictionary in Python is an unordered collection of data values, used to store data values like a map, which unlike other Data Types that hold only single value as an element, Dictionary holds **key:value** pair.

Dictonaries are like Hash Tables used in other languages.


```
# Make a dictionary with {} and : to signify a key and a value
my_dict = {'key1':'value1','key2':'value2'}
```


```
# Call values by their key
my_dict['key2']
```


Its important to note that dictionaries are **very flexible** in the data types they can hold.

```
my_dict = {'key1':123,'key2':[12,23,33],'key3':['item0','item1','item2']}



# Let's call items from the dictionary
my_dict['key3']

> ['item0', 'item1', 'item2']



# Can call an index on that value
my_dict['key3'][0]

> 'item0'

```


To see the power and flexibility of Python lets see nested dictonaries.

```
# Dictionary nested inside a dictionary nested inside a dictionary
d = {'key1':{'nestkey':{'subnestkey':'value'}}}


# Let's see how we can grab that value:

# Keep calling the keys
d['key1']['nestkey']['subnestkey']

> 'value'
```


### Dictonary Methods

```
# Create a typical dictionary
d = {'key1':1,'key2':2,'key3':3}



# Method to return a list of all keys 
d.keys()

> dict_keys(['key1', 'key2', 'key3'])



# Method to grab all values
d.values()

> dict_values([1, 2, 3])



# Method to return tuples of all items
d.items()

> dict_items([('key1', 1), ('key2', 2), ('key3', 3)])

```


### Tuples

In Python tuples are very similar to lists, however, unlike lists they are immutable meaning they can not be changed.

The construction of a tuples use () with elements separated by commas.

```
# Create a tuple
t = (1,2,3)

t

> (1, 2, 3)
```

```
# Check len just like a list

len(t)

> 3
```

*Can also **mix object types***

```
t = ('one',2)

# Show
t

> ('one', 2)
```


*Use **indexing** just like we did in lists*
```
t[0]

> 'one'
```

***Slicing** just like a list*
```
t[-1]

> 2
```


### Tuple Methods

Tuple has two built-in methods.

***index***

```
# Use .index to enter a value and return the index
t.index('one')

> 0
```

***count***

```
# Use .count to count the number of times a value appears
t.count('one')
```

### Tuples are Immutable!
```
t[0]= 'change'

> TypeError: 'tuple' object does not support item assignment

```

Because of this immutability, tuples can't grow. Once a tuple is made we can not add to it.

```
t.append('nope')

> AttributeError: 'tuple' object has no attribute 'append'
```

### Use of Tuple

If in your program you are passing around an object and need to make sure it does not get changed, then a tuple becomes your solution. It provides a convenient source of data integrity.


## Sets 

Sets are an unordered collection of unique elements. 

```
x = set()

# We add to sets with the add() method
x.add(1)

#Show
x

> {1}


# Add a different element
x.add(2)

# Try to add the same element
x.add(1)


#Show
x

> {1, 2}
```

**Notice** how it won't place another 1 there. That's because a set is only concerned with unique elements! 



We can cast a list with multiple repeat elements to a set to get the unique elements. For example:

```
# Create a list with repeats
list1 = [1,1,2,2,3,4,5,6,1,1]


# Cast as set to get unique values
set(list1)

> {1, 2, 3, 4, 5, 6}
```


## Booleans 

```
# Boolean values are primitives (Note: the capitalization)
True  # => True
False  # => False

# negate with not
not True   # => False
not False  # => True

# Boolean Operators
# Note "and" and "or" are case-sensitive
True and False  # => False
False or True   # => True
```


![alt text](https://github.com/ishpreet-singh/python3-workshop/blob/master/assets/comparison-operator-table.png)


## File Handling

Python uses file objects to interact with external files on your computer. 


Let's suppose **test.txt** exist in the directory with contents, 

`Hello, this is a quick test file.`


```
myfile = open('test.txt')

# We can now read the file
my_file.read()



# But what happens if we try to read it again?
my_file.read()

> ''

```

This happens because you can imagine the reading "cursor" is at the end of the file after having read it. So there is nothing left to read. We can reset the "cursor" like this:

```
# Seek to the start of file (index 0)
my_file.seek(0)

> 0
```

```
# Now read again
my_file.read()

> 'Hello, this is a quick test file.'
```


### Writing to a File

```
# Add a second argument to the function, 'w' which stands for write.
# Passing 'w+' lets us read and write to the file

my_file = open('test.txt','w+')

```

Opening a file with 'w' or 'w+' truncates the original, meaning that anything that was in the original file is deleted!

```
my_file.write('This is a new line')
```


# Python Statements

## if, elif, else Statements

```
if case1:
    perform action1
elif case2:
    perform action2
else: 
    perform action3
```


```
loc = 'Bank'

if loc == 'Auto Shop':
    print('Welcome to the Auto Shop!')
elif loc == 'Bank':
    print('Welcome to the bank!')
else:
    print('Where are you?')
```


> **Indentation**: It is important to keep a good understanding of how indentation works in Python to maintain the structure and order of your code. We will touch on this topic again when we start building out functions!


# Loops

## For Loop

for loop acts as an iterator in Python; it goes through items that are in a sequence or any other iterable item. 

```
for item in object:
    statements to do stuff
```


Iterating through a list
```
# We'll learn how to automate this sort of list in the next lecture
list1 = [1,2,3,4,5,6,7,8,9,10]


for num in list1:
    print(num)


1
2
3
4
5
6
7
8
9
10
```


```
# Start sum at zero
list_sum = 0 

for num in list1:
    list_sum += num

print(list_sum)
> 55
```


Tuples have a special quality when it comes to for loops. If you are iterating through a sequence that contains tuples, the item can actually be the tuple itself, this is an example of tuple unpacking.

```
list2 = [(2,4),(6,8),(10,12)]


for tup in list2:
    print(tup)


> 
(2, 4)
(6, 8)
(10, 12)
```

During the for loop we will be unpacking the tuple inside of a sequence and we can access the individual items inside that tuple!


```
# Now with unpacking!
for (t1,t2) in list2:
    print(t1)

> 
2
6
10
```


```
d = {'k1':1,'k2':2,'k3':3}


for item in d:
    print(item)

>
k1
k2
k3
```

We can perform dictionary unpacking to separate keys and values just as we did in the previous examples.
```
# Dictionary unpacking
for k,v in d.items():
    print(k, v)


>
k1 1
k2 2
k3 3
```


Remember that dictionaries are unordered, and that keys and values come back in arbitrary order. You can obtain a sorted list using `sorted()`

```
sorted(d.values())


> [1, 2, 3]
```


## While Loop

The while statement in Python is one of most general ways to perform iteration. 


```
while test:
    code statements
else:
    final code statements
```


Example:

```
x = 0
while x < 5:
    print('x: ', x)
    x+=1

> 
x:  0
x:  1
x:  2
x:  3
x:  4
```

### Range

The range function allows you to quickly generate a list of integers, this comes in handy a lot, so take note of how to use it! There are 3 parameters you can pass, a start, a stop, and a step size.


```
list(range(0,11))

> 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10
# Notice how 11 is not included, up to but not including 11, just like slice notation!


# Third parameter is step size!
list(range(0,11,2))

> [0, 2, 4, 6, 8, 10]
```

Note that this is a generator function


### Enumerate

enumerate() method adds a counter to an iterable and returns it in a form of enumerate object.

```
for i,letter in enumerate('abcde'):
    print("At index {} the letter is {}".format(i,letter))


>
At index 0 the letter is a
At index 1 the letter is b
At index 2 the letter is c
At index 3 the letter is d
At index 4 the letter is e
```


Notice the format enumerate actually returns, let's take a look by transforming it to a list()
```
list(enumerate('abcde'))

[(0, 'a'), (1, 'b'), (2, 'c'), (3, 'd'), (4, 'e')]
```


### Zip

To zip two list together

```
mylist1 = [1,2,3,4,5]
mylist2 = ['a','b','c','d','e']


list(zip(mylist1,mylist2))

> [(1, 'a'), (2, 'b'), (3, 'c'), (4, 'd'), (5, 'e')]
```


### In

To Check the membership of object

```
'x' in ['x','y','z']
>
True

'x' in [1,2,3]
>
False
```


### Random

Python comes with a built in random library.

Two of the most popular functions of random library are:

* *shuffle*

This shuffles the list "in-place" meaning it won't return anything, instead it will effect the list passed

```
from random import shuffle

shuffle(mylist)
```


* *randint*
Return random integer in range [a, b], including both end points.

```
from random import randint

randint(0,100)
```


* ***input***


```
input('Enter Something into this box: ')
```


## Functions
Functions are the building blocks to construct larger and larger amounts of code to solve problems.

A Function is apiece of code that groups together a set of statements so they can be run more than once.

They can also let us specify parameters that can serve as inputs to the functions.


```
def name_of_function(arg1,arg2):
    '''
    This is where the function's Document String (docstring) goes
    '''
    # Do stuff here
    # Return desired result
```


*A simple print 'hello' function*

```
def say_hello():
    print('hello')

say_hello()


> hello
```

*A function to add numbers*

```
def add_num(num1,num2):
    return num1+num2


add_num(2, 5)

> 7
```

*A function to check if number is Prime or not*

```
import math

def is_prime2(num):
    '''
    Method to check if number is prime
    '''
    for i in range(2, int(math.sqrt(num)) + 1):
        if num % i == 0:
            return False
    return True


is_prime2(18)
>
False


is_prime2(17)
>
True

```

## Args and Kwargs

***Args**

When a function parameter starts with an asterisk, it allows for an arbitrary number of arguments, and the function takes them in as a tuple of values. 

```
def myfunc(*args):
    return sum(args)*.05

myfunc(40,60,20)

>
6.0
```

****Kwargs**

Similarly, Python offers a way to handle arbitrary numbers of keyworded arguments. Instead of creating a tuple of values, **kwargs builds a dictionary of key/value pairs.


```
def myfunc(**kwargs):
    if 'fruit' in kwargs:
        print(f"My favorite fruit is {kwargs['fruit']}")  # review String Formatting and f-strings if this syntax is unfamiliar
    else:
        print("I don't like fruit")
        
    
myfunc(fruit='pineapple')
> My favorite fruit is pineapple


myfunc()
> I don't like fruit
```


## Lambda Expressions, Map, and Filter

### Map Function

The map function allows you to "map" a function to an iterable object. That is to say you can quickly call the same function to every item in an iterable, such as a list.


```
def square(num):
    return num**2

my_nums = [1,2,3,4,5]


# To get the results, either iterate through map() 
# or just cast to a list

list(map(square,my_nums))

> [1, 4, 9, 16, 25]
```


### Filter Function

The filter function returns an iterator yielding those items of iterable for which function(item) is true.

Meaning you need to filter by a function that returns either True or False.


```
def check_even(num):
    return num % 2 == 0

nums = [0,1,2,3,4,5,6,7,8,9,10]

list(filter(check_even,nums))

> [0, 2, 4, 6, 8, 10]
```


### Lambda expression

Lambda expressions allow us to create "anonymous" functions. 

This basically means we can quickly make ad-hoc functions without needing to properly define a function using def.

Function objects returned by running lambda expressions work exactly the same as those created and assigned by defs.

**lambda's body is a single expression, not a block of statements.**


*Lets slowly break down a lambda expression by deconstructing a function:*
```
def square(num):
    result = num**2
    return result

square(2)

> 4
```

We could simplify it:
```
def square(num):
    return num**2
```


We could actually even write this all on one line.
```
def square(num): return num**2
```

This is the form a function that a lambda expression intends to replicate. A lambda expression can then be written as:

```
lambda num: num ** 2
```


```
my_nums = [1,2,3,4,5]

list(map(lambda num: num ** 2, my_nums))

>[1, 4, 9, 16, 25]
```


```
my_nums = [1,2,3,4,5]

list(filter(lambda n: n % 2 == 0,nums))

>[0, 2, 4, 6, 8, 10]
```

## Object Oriented Programming

### Objects

In Python, everything is an object.

```
print(type([]))
print(type(()))

>
<class 'list'>
<class 'tuple'>
```


### Class
User defined objects are created using the class keyword. 

```
# Create a new object type called Sample
class Sample:
    pass

# Instance of Sample
x = Sample()

print(type(x))

>
<class '__main__.Sample'>
```

By convention we give classes a name that starts with a capital letter. Note how x is now the reference to our new instance of a Sample class. In other words, we instantiate the Sample class.


An **attribute** is a characteristic of an object. 

A **method** is an operation we can perform with the object.


The syntax for creating an attribute is:

```
self.attribute = something
```

There is a special method called:

```
__init__()
```



This method is used to initialize the attributes of an object.

```
class Dog:
    def __init__(self,breed):
        self.breed = breed
        
sam = Dog(breed='Lab')
frank = Dog(breed='Huskie')



sam.breed
> 'Lab'


frank.breed
> 'Huskie'

```


### Methods

Methods are functions defined inside the body of a class. They are used to perform operations with the attributes of our objects.


```
class Circle:
    pi = 3.14

    # Circle gets instantiated with a radius (default is 1)
    def __init__(self, radius=1):
        self.radius = radius 
        self.area = radius * radius * Circle.pi

    # Method for resetting Radius
    def setRadius(self, new_radius):
        self.radius = new_radius
        self.area = new_radius * new_radius * self.pi

    # Method for getting Circumference
    def getCircumference(self):
        return self.radius * self.pi * 2


c = Circle()

print('Radius is: ',c.radius)
print('Area is: ',c.area)
print('Circumference is: ',c.getCircumference())


>
Radius is:  1
Area is:  3.14
Circumference is:  6.28
```


## Inheritance

Inheritance is the ability of class to inherit the properties of an existing class. 

The class which derives the property if called Derived Class.

The class from which it derives its property is called Base class.

It is used to represent *is a kind of relationship*.


```
class Animal:
    def __init__(self):
        print("Animal created")

    def whoAmI(self):
        print("Animal")

    def eat(self):
        print("Eating")


class Dog(Animal):
    def __init__(self):
        Animal.__init__(self)
        print("Dog created")

    def whoAmI(self):
        print("Dog")

    def bark(self):
        print("Woof!")
```


```
d = Dog()

>
Animal created
Dog created


d.whoAmI()
> Dog


d.eat()
> Eating


d.bark()
> Woof!

```


## Polymorphism


Polymorphism is the ability to be represented in more than one form.

Polymorphism refers to the way in which different object classes can share the same method name, and those methods can be called from the same place even though a variety of different objects might be passed in.


```
class Dog:
    def __init__(self, name):
        self.name = name

    def speak(self):
        return self.name+' says Woof!'
    
class Cat:
    def __init__(self, name):
        self.name = name

    def speak(self):
        return self.name+' says Meow!' 
    

niko = Dog('Niko')
felix = Cat('Felix')


print(niko.speak())
print(felix.speak())
```


Here we have a Dog class and a Cat class, and each has a .speak() method. When called, each object's .speak() method returns a result unique to the object.


```
def pet_speak(pet):
    print(pet.speak())

pet_speak(niko)
pet_speak(felix)

> 
Niko says Woof!
Felix says Meow!

```

## Time to Practice

* [Practice](https://github.com/ishpreet-singh/python3-workshop/tree/master/practice)


----

## Some Resources to start your Python Journey

* https://docs.python.org/3/ 
* https://github.com/promehul/python_assignment-1/blob/master/Learn%20Python%203%20the%20Hard%20Way.pdf
* https://developers.google.com/edu/python 
* https://learnxinyminutes.com/docs/python3/
* https://www.udemy.com/course/learn-python-3-from-beginner-to-advanced/ 
* https://www.youtube.com/watch?v=yE9v9rt6ziw 
* https://www.kaggle.com/learn/python



## References

* https://docs.python.org/3/ 
* https://github.com/Pierian-Data/Complete-Python-3-Bootcamp
* https://learnxinyminutes.com/docs/python3/
* https://developers.google.com/edu/python 
* https://www.youtube.com/channel/UCWv7vMbMWH4-V0ZXdmDpPBA

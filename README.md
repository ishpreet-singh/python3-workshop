# Python Workshop

## Why Python? What's the hype?

## Some History of Python

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

### Indexing and Slicing

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


----

# References

* https://github.com/Pierian-Data/Complete-Python-3-Bootcamp
* https://learnxinyminutes.com/docs/python3/
* 

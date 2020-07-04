
# course_2_assessment_4

-------------------------

# Description: Assessment for Functions lesson

-----------------------------

# Questions

------------------------------

Write a function called int_return that takes an integer as input and returns the same integer.

```
def int_return(x):

    return x
```

----------------------------------------------------------

Write a function called add that takes any number as its input and returns that sum with 2 added.

```
def add(x):

    return x + 2
```

-----------------------------------------------

Write a function called change that takes any string, adds “Nice to meet you!” to the end of the argument given, and returns that new string.

```
def change(x):

    words = "Nice to meet you!"

    newstring = x + words

    return newstring
```
    
------------------------------------------------------

Write a function, accum, that takes a list of integers as input and returns the sum of those integers.

```
def accum(x):

    tot = 0

    for i in x:

        tot = tot + i

    return tot
```

------------------------------------------------

Write a function, length, that takes in a list as the input. If the length of the list is greater than or equal to 5, return “Longer than 5”. If the length is less than 5, return “Less than 5”.

```
def length(x):

    c = 0

    y = "Less than 5"

    for i in x:

        c = c + 1

    if c > 4:

        y = "Longer than 5"

    return y
```

-------------------------------------------------------


You will need to write two functions for this problem. The first function, divide that takes in any number and returns that same number divided by 2. The second function called sum should take any number, divide it by 2, and add 6. It should return this new number. You should call the divide function within the sum function. Do not worry about decimals.

```
def divide(x):

    z = x / 2 

    return z

def sum(x):

    z = divide(x) + 6

    return z
```

------------------------------------------------------------------------

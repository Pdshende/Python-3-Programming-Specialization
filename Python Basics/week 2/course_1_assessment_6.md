# course_1_assessment_6

# Due: 2018-11-25 01:19:00

# Score: 9.0 of 9 = 100.0%
Description: Assessment for Way of Programmer Week 2 lesson.

--------------------------------------------------------------------------

Write one for loop to print out each character of the string my_str on a separate line.

1
my_str = "MICHIGAN" <br>

-----------------------------------------------
````
for i in range(len(my_str)):
    print(my_str[i]) 
    
````

---------------------------------------------------

Write one for loop to print out each element of the list several_things. Then, write another for loop to print out the TYPE of each element of the list several_things. To complete this problem you should have written two different for loops, each of which iterates over the list several_things, but each of those 2 for loops should have a different result.

1
several_things = ["hello", 2, 4, 6.0, 7.5, 234352354, "the end", "", 99]


```
for element in several_things:
    print(element)
    
for element in several_things:
    print(type(element))
```

-------------------------------------------------------------------------

Write code that uses iteration to print out the length of each element of the list stored in str_list.

1
str_list = ["hello", "", "goodbye", "wonderful", "I love Python"]



```
# Write your code here.
for i in str_list:
    print(len(i))
```
------------------------------------------------------------------------------------

Write code to count the number of characters in original_str using the accumulation pattern and assign the answer to a variable num_chars. Do NOT use the len function to solve the problem (if you use it while you are working on this problem, comment it out afterward!)

1
original_str = "The quick brown rhino jumped over the extremely lazy fox."

```
num_chars = 0
for i in original_str:
    num_chars = num_chars+1
print(num_chars)    
```
----------------------------------------------------------------------------------

addition_str is a string with a list of numbers separated by the + sign. Write code that uses the accumulation pattern to take the sum of all of the numbers and assigns it to sum_val (an integer). (You should use the .split("+") function to split by "+" and int() to cast to an integer).

1
addition_str = "2+5+10+20"

```
numbers=addition_str.split("+")

sum_val=0

for num in numbers:
    sum_val=sum_val+int(num)
print(sum_val)
```
------------------------------------------------------------------------

week_temps_f is a string with a list of fahrenheit temperatures separated by the , sign. Write code that uses the accumulation pattern to compute the average (sum divided by number of items) and assigns it to avg_temp. Do not hard code your answer (i.e., make your code compute both the sum or the number of items in week_temps_f) (You should use the .split(",") function to split by "," and float() to cast to a float).


week_temps_f = "75.1,77.7,83.2,82.5,81.0,79.5,85.7"

```
ans = week_temps_f.split(",")

sum1 = 0
for i in ans:
    sum1 = sum1+ float(i)
avg_temp = sum1/len(ans)
print(avg_temp)
```

------------------------------------------------------------------------------

Write code to create a list of numbers from 0 to 67 and assign that list to the variable nums. Do not hard code the list.


```
nums=list(range(68))
```
--------------------------------------------------------------------

Write code to create a list of word lengths for the words in original_str using the accumulation pattern and assign the answer to a variable num_words_list. (You should use the len function).


original_str = "The quick brown rhino jumped over the extremely lazy fox"

```
words=original_str.split()

num_words_list=[]

for word in words:
    num_words_list.append(len(word))

print(num_words_list)
```
---------------------------------------------------------------------------------

Create an empty string and assign it to the variable lett. Then using range, write code such that when your code is run, lett has 7 b’s ("bbbbbbb").

```
lett=""

for i in range(7):
    lett=lett+'b'

print(lett)
```
-----------------------------------------------------------------------------

Write a program that uses the turtle module and a for loop to draw something. It doesn’t have to be complicated, but draw something different than we have done in the past. (Hint: if you are drawing something complicated, it could get tedious to watch it draw over and over. Try setting .speed(10) for the turtle to draw fast, or .speed(0) for it to draw super fast with no animation.)

```
import turtle
wan  = turtle.Screen()
p = turtle.Turtle()
dis = 50
ang = 70
p.speed(10)
for i in range(40):
    p.forward(dis)
    p.right(ang)
    ang = ang+10
 ```   

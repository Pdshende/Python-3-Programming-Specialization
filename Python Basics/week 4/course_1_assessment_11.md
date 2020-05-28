# Questions
# Score: 1.0 / 1
# Comment: autograded

-------------------------------------------------------------------------------------------------

Which of these is a correct reference diagram following the execution of the following code?
```
lst = ['mercury', 'venus', 'earth', 'mars', 'jupiter', 'saturn', 'uranus', 'neptune', 'pluto']
lst.remove('pluto')
first_three = lst[:3]
```
![pict3](https://github.com/Pdshende/Python-3-Programming-Specialization/blob/master/picture/Screenshot%20from%202020-05-28%2023-53-58.png)

A. I.

------------------------------------------------------------------------------------------------

What will be the value of a after the following code has executed?

```
a = ["holiday", "celebrate!"]
quiet = a
quiet.append("company")
The value of a will be
```
```
['holiday', 'celebrate!', 'company']
```
------------------------------------------------------------------------------------------------

Could aliasing cause potential confusion in this problem?

```
b = ['q', 'u', 'i']
z = b
b[1] = 'i'
z.remove('i')
print(z)
```
```
A. yes
```
---------------------------------------------------------------------------------------

Given that we want to accumulate the total sum of a list of numbers, which of the following accumulator patterns would be appropriate?

```
1
nums = [4, 5, 2, 93, 3, 5]
s = 0
for n in nums:
    s = s + 1
```
```
2
nums = [4, 5, 2, 93, 3, 5]
s = 0
for n in nums:
    s = n + n
```
```
3
nums = [4, 5, 2, 93, 3, 5]
s = 0
for n in nums:
    s = s + n
```
```
C. III.
```
------------------------------------------------------------------------------

Given that we want to accumulate the total number of strings in the list, which of the following accumulator patterns would be appropriate?

```
1
lst = ['plan', 'answer', 5, 9.29, 'order, items', [4]]
s = 0
for n in lst:
    s = s + n
```
```
2
lst = ['plan', 'answer', 5, 9.29, 'order, items', [4]]
for item in lst:
    s = 0
    if type(item) == type("string"):
        s = s + 1
```
```
3
lst = ['plan', 'answer', 5, 9.29, 'order, items', [4]]
s = ""
for n in lst:
    s = s + n
```
```
4
lst = ['plan', 'answer', 5, 9.29, 'order, items', [4]]
s = 0
for item in lst:
    if type(item) == type("string"):
        s = s + 1
```
```
D. 4.
```
---------------------------------------------------------------------------------------
Which of these are good names for an accumulator variable? Select as many as apply.

```
C. total
D. accum
```

----------------------------------------------------------------------------------------


Which of these are good names for an iterator (loop) variable? Select as many as apply.

```
A. item
C. elem
D. char
```
----------------------------------------------------------------------------------------

Which of these are good names for a sequence variable? Select as many as apply.

```
A. num_lst
C. sentence
D. names
```
------------------------------------------------------------------------------------

Given the following scenario, what are good names for the accumulator variable, iterator variable, and sequence variable? You are writing code that uses a list of sentences and accumulates the total number of sentences that have the word ‘happy’ in them.

```
D. accumulator variable: total | iterator variable: sentence |sequence variable: sentence_lst

```
----------------------------------------------------------------------------------




































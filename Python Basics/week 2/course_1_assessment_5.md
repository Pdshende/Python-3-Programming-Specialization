# course_1_assessment_5
# Due: 2018-11-25 01:17:00
# Score: 8.0 of 8 = 100.0%
# Description: Assessment for Lists and Strings lesson.

------------------------------------------------------------------------
Questions
Score: 1.0 / 1
Comment: autograded

sequences-10-1: What will the output be for the following code?<br>

let = "z"<br>
let_two = "p"<br>
c = let_two + let<br>
m = c*5<br>
print(m)<br>

C. pzpzpzpzpz<br>

------------------------------------------------------------

Write a program that extracts the last three items in the list sports and assigns it to the variable last. Make sure to write your code so that it works no matter how many items are in the list.

1
sports = ['cricket', 'football', 'volleyball', 'baseball', 'softball', 'track and field', 'curling', 'ping pong', 'hockey']<br>


sports = ['cricket', 'football', 'volleyball', 'baseball', 'softball', 'track and field', 'curling', 'ping pong', 'hockey']
<br>
a = sports[len(sports) - 2]<br>
b = sports[len(sports) - 1]<br>
c = sports[len(sports) - 3]<br>
last = [ 'curling', 'ping pong', 'hockey']<br>

------------------------------------------------------------------------

Write code that combines the following variables so that the sentence “You are doing a great job, keep it up!” is assigned to the variable message. Do not edit the values assigned to by, az, io, or qy.

1
by = "You are"<br>
2
az = "doing a great "<br>
3
io = "job"<br>
4
qy = "keep it up!"<br>


message = by+az+io+qy<br>

---------------------------------------------------------------------------------------

sequences-10-2: What will the output be for the following code?

ls = ['run', 'world', 'travel', 'lights', 'moon', 'baseball', 'sea']<br>
new = ls[2:4]<br>
print(new)<br>

C. ['travel', 'lights']<br>

------------------------------------------------------------------------

sequences-10-3: What is the type of m?<br>

l = ['w', '7', 0, 9]<br>
m = l[1:2]<br>


D. list

---------------------------------------------------------------------

sequences-10-4: What is the type of m?<br>

l = ['w', '7', 0, 9]<br>
m = l[1]<br>

A. string<br>

--------------------------------------------------------------------------------


sequences-10-5: What is the type of x?<br>

b = "My, what a lovely day"<br>
x = b.split(',')<br>

D. list

--------------------------------------------------------------------------------


sequences-10-6: What is the type of a?<br>

b = "My, what a lovely day"<br>
x = b.split(',')<br>
z = "".join(x)<br>
y = z.split()<br>
a = "".join(y)<br>

A. string


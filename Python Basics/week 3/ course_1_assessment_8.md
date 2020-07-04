# Questions
# Score: 1.0 / 1
# Comment: autograded

-----------------------------------------------------------------------------------

seqmut-1-5: Could aliasing cause potential confusion in this problem?

b = ['q', 'u', 'i']
z = b
b[1] = 'i'
z.remove('i')
print(z)

```
A. yes
```

-----------------------------------------------------------------------------------------



seqmut-1-6: Could aliasing cause potential confusion in this problem?

sent = "Holidays can be a fun time when you have good company!"
phrase = sent
phrase = phrase + " Holidays can also be fun on your own!"

```
B. no
```
----------------------------------------------------------------------------------


seqmut-1-1: Which of these is a correct reference diagram following the execution of the following code?

lst = ['mercury', 'venus', 'earth', 'mars', 'jupiter', 'saturn', 'uranus', 'neptune', 'pluto']
lst.remove('pluto')
first_three = lst[:3]

![pic1](https://github.com/Pdshende/Python-3-Programming-Specialization/blob/master/picture/Screenshot%20from%202020-05-28%2023-06-21.png)

```
A. I.
```

--------------------------------------------------------------------------------------


seqmut-1-7: Which of these is a correct reference diagram following the execution of the following code?

x = ["dogs", "cats", "birds", "reptiles"]
y = x
x += ['fish', 'horses']
y = y + ['sheep']

![pic2](https://github.com/Pdshende/Python-3-Programming-Specialization/blob/master/picture/Screenshot%20from%202020-05-28%2023-09-45.png)

```
D. IV.
```
------------------------------------------------------------------------------------------------------


seqmut-1-8: Which of these is a correct reference diagram following the execution of the following code?

sent = "The mall has excellent sales right now."
wrds = sent.split()
wrds[1] = 'store'
new_sent = " ".join(wrds)

![pic3](https://github.com/Pdshende/Python-3-Programming-Specialization/blob/master/picture/Screenshot%20from%202020-05-28%2023-10-13.png)

```
D. IV.
```

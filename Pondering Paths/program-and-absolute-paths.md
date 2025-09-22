# Intro to Arguments
The challenge requires you to invoke a program using an abolsute path.

## My Solve
**Flag:**  'pwn.college{sJQHX54VbKP6vXWr1XbV0figb0X.QX1QTN0wSM0AzNzEzW}'

We execute the '/challenge/run' to invoke the program as this is an absolute path. This works because the name of the program is run which is stored in the challenge directory. 

```

hacker@paths~program-and-absolute-paths:~$ /challenge/run
Correct!!!
/challenge/run is an absolute path! Here is your flag:
pwn.college{sJQHX54VbKP6vXWr1XbV0figb0X.QX1QTN0wSM0AzNzEzW}

```

## What I learned
I learned how to invoke programs that may have directories that are a little complicated, and what exactly is an absolute path and how it is implemented.

## References
Nil.

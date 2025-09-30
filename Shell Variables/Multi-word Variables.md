# Multi-word Variables
The challenge requires you to assign a mutli-word value to a variable.

## My Solve
**Flag:**  'pwn.college{8eMTW2qYJAtKxS-Ry-jl-7Jtspv.QXwYTN0wSM0AzNzEzW}'

We simply need to use the 'PWN="COLLEGE YEAH"' command to assign a multi-word value to the 'PWN' variable.

```
hacker@variables~multi-word-variables:~$ PWN="COLLEGE YEAH"
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{8eMTW2qYJAtKxS-Ry-jl-7Jtspv.QXwYTN0wSM0AzNzEzW}
```

## What I learned
I learned that we can't use spaces normally while assigning values to a variable, be it around the '=' operator or be it a multi-word varaible. 
As such, we must quote "" the multi-word variable to successfully asssign it the value without the shell misinterpreting our command.

## References
Nil.

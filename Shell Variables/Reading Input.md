# Reading Input
The challenge needs you to take an input for the PWN variable.

## My Solve
**Flag:**  'pwn.college{8oOLO5f9yauTuTEPDn1DA3t2EMI.QX4cTN0wSM0AzNzEzW}'

First, we use the 'read -p "Enter value for PWN: " PWN' command which takes input for the variable PWN.
Then, we enter the value 'COLLEGE' for the variable PWN, which gives us the flag.

```
hacker@variables~reading-input:~$ read -p "Enter value for PWN: " PWN
Enter value for PWN: COLLEGE
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{8oOLO5f9yauTuTEPDn1DA3t2EMI.QX4cTN0wSM0AzNzEzW}
```

## What I learned
I learned how to take the input from the user, that is us in this case. 
I learned that the '-p' operator specifies that we want to read a prompt.

## References
Nil.

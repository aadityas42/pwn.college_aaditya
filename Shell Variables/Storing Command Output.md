# Storing Command Output
The challenge needs you to store the output of a command directly in a variable

## My Solve
**Flag:**  'pwn.college{AoIrjVbClE_xIp41M08V2M24HIp.QX1cDN1wSM0AzNzEzW}'

First, we use the 'PWN=$(/challenge/run)' to store the output of the command '/challenge/run' in the vraible 'PWN'.
Then, we use 'echo "$PWN"' to output the contents of the variable that is, our flag.

```
hacker@variables~storing-command-output:~$ PWN=$(/challenge/run)
Congratulations! You have read the flag into the PWN variable. Now print it out 
and submit it!
hacker@variables~storing-command-output:~$ echo "$PWN"
pwn.college{AoIrjVbClE_xIp41M08V2M24HIp.QX1cDN1wSM0AzNzEzW}
```

## What I learned
I learned how to store the output of a command directly in a variable using Command Substitution.
I also learned that we can use the '' operator instead of $() to store the output, although it is a older format and generally not preferred because it is less readable.

## References
Nil.

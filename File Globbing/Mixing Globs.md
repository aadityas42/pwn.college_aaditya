# Mixing Globs
The challenge puts all the knowledge we learnt about globbing to the test.

## My Solve
**Flag:**  'pwn.college{MQtRxycgiMM7gyt0tGITpc8utDE.QX1IDO0wSM0AzNzEzW}'

We first switch our cwd to files, and then use our argument as '[cep]*'. In this, the first part, '[cep]' ensures that we look for files that start with 'c' or 'e' or 'p'  and the second part ensures to complete the remaingin pattern.

```
hacker@globbing~mixing-globs:~$ cd /challenge/files
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run [cep]*
You got it! Here is your flag!
pwn.college{MQtRxycgiMM7gyt0tGITpc8utDE.QX1IDO0wSM0AzNzEzW}
```

## What I learned
I learned how to apply all of the thing I learnt so far about globbing, like a combination of the '*' and '[]' operators to solve a more complicated challenge which is closer to a real world scenario where multiple commands need to be applied together.

## References
Nil.

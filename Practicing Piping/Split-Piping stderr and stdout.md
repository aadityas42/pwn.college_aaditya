# Split-Piping stderr and stdout
The challenge requires you to pipe the output stderr to one program and stdout to another.

## My Solve
**Flag:**  'pwn.college{AfEHCJrOpesFgzZQvco3ToGFTGV.QXxQDM2wSM0AzNzEzW}'

We execute the '/challenge/hack 2> >(/challenge/the) | /challenge/planet' command. 
The first part with the '2>' and '>' operators, the '2>' operator is used to redirect the error, and the '>()' operator is the process substitution. 
The second part with '|' is just used to pipe the output to '/challenge/planet.

```
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack 2> >(/challenge/the) | /challenge/planet
Congratulations, you have learned a redirection technique that even experts 
struggle with! Here is your flag:
pwn.college{AfEHCJrOpesFgzZQvco3ToGFTGV.QXxQDM2wSM0AzNzEzW}
```

## What I learned
I learned how to pipe output and error, both at once to two different locations using a combination of the '>()','2>' and '|' operators.

## References
Nil.

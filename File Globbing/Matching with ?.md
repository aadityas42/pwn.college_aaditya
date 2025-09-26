# Matching with ?
The challenge requires us to use the '?' operator to match missing charecters.

## My Solve
**Flag:**  'pwn.college{EvbzdQMpC_PH38Tq43E_V8VX2rs.QXyIDO0wSM0AzNzEzW}'

We execute the 'cd /?ha??enge' command, using a '?' in place of 'c' and '??' in place of 'll' to switch our working directory to challenge, and then run the program to get flag.

```
hacker@globbing~matching-with-:~$ cd /?ha??enge
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{EvbzdQMpC_PH38Tq43E_V8VX2rs.QXyIDO0wSM0AzNzEzW}
```

## What I learned
I learned that the '?' operator is different from the '*' operator in the sense that it can only match one charecter compared to '*' which can match multiple charecters.

## References
Nil.

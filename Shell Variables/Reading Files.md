# Reading Files
The challenge needs you to take an input for the PWN variable directly from the output of a file.

## My Solve
**Flag:**  'pwn.college{UD0fDA42xB2ckwqEKvhUxt_wuVQ.QXwIDO0wSM0AzNzEzW}'

First, we use the 'read PWN < /challenge/read_me' command which assigns the contents of the file to the 'PWN' variable directly without needing to use the echo command.

```
hacker@variables~reading-files:~$ read PWN < /challenge/read_me
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{UD0fDA42xB2ckwqEKvhUxt_wuVQ.QXwIDO0wSM0AzNzEzW}
```

## What I learned
I learned how to use contents fo a file as the input for a variable, without needing to use the echo command as it doesn't make sense to run a whole program just to read the file using echo.

## References
Nil.

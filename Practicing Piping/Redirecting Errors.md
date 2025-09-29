# Redirecting Errors
The challenge requires you to redirect two parts of the program run to two different locations.

## My Solve
**Flag:**  'pwn.college{gGINkUrT1SHSEd8pit4tWKdJ8Ai.QX3YTN0wSM0AzNzEzW}'

We execute the '/challenge/run > myflag 2> instructions' command to redirect the output, that is the flag to 'myflag' and the errors to 'instructions' file. using the '>' and '2>' operators. Then we can cat 'myflag' to get the flag.

```
hacker@piping~redirecting-errors:~$ /challenge/run > myflag 2> instructions
hacker@piping~redirecting-errors:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{gGINkUrT1SHSEd8pit4tWKdJ8Ai.QX3YTN0wSM0AzNzEzW}
```

## What I learned
I learned that we can redirect both the output and error of a command to two different locations at the same time.

## References
Nil.

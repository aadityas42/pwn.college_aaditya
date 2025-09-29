# Redirecting Input
The challenge requires you to redirect the output of a file and then an input.

## My Solve
**Flag:**  'pwn.college{UqPjYOnENW5-aun6txMRQry-Nuk.QXwcTN0wSM0AzNzEzW}'

We execute the 'echo COLLEGE > PWN' command to create the 'PWN' file and store the string 'COLLEGE' in it. Then we take the file 'PWN', and redirect it as an input using the command '/challenge/run < PWN' to get the flag.

```
hacker@piping~redirecting-input:~$ echo COLLEGE > PWN
hacker@piping~redirecting-input:~$ /challenge/run < PWN
Reading from standard input...
Correct! You have redirected the PWN file into my standard input, and I read 
the value 'COLLEGE' out of it!
Here is your flag:
pwn.college{UqPjYOnENW5-aun6txMRQry-Nuk.QXwcTN0wSM0AzNzEzW}
```

## What I learned
I learned that we can redirect both the output and input as well for any given command. As such, I learned how to use a combination of the two and that this can lead to a lot of interesting results when used correctly.

## References
Nil.

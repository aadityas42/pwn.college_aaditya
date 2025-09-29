# Redirecting Output
The challenge requires you to redirect the output of the echo command to another file.

## My Solve
**Flag:**  'pwn.college{E8coE3dKBrwgcl7syM_8jducnPV.QX0YTN0wSM0AzNzEzW}'

We execute the 'echo PWN > COLLEGE' command this command basically redirects the output 'PWN' to the file 'COLLEGE', which gives  us the flag.

```
hacker@piping~redirecting-output:~$ echo PWN > COLLEGE
Correct! You successfully redirected 'PWN' to the file 'COLLEGE'! Here is your 
flag:
pwn.college{E8coE3dKBrwgcl7syM_8jducnPV.QX0YTN0wSM0AzNzEzW}

```

## What I learned
I learned that we can redirect outputs to other file locations, in this case we use the '>' operator coupled with the echo command to do the same. After this, we can use a command like 'cat' to output it from the new location.

## References
Nil.


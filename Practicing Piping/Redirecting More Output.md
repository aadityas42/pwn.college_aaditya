# Redirecting More Output
The challenge requires you to redirect the output of the other commands to another file.

## My Solve
**Flag:**  'pwn.college{IW3ceILpE87EM6TDQQqGuO3WH_c.QX1YTN0wSM0AzNzEzW}'

We execute the '/challenge/run > myflag' command. This command basically redirects the output of '/challenge/run' which is the flag, to the file 'myflag', which gives  us the flag on catting it.

```
hacker@piping~redirecting-more-output:~$ /challenge/run > myflag
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : myflag
[INFO] - the challenge will output a reward file if all the tests pass : /flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /flag file.

[TEST] You should have redirected my stdout to a file called myflag. Checking...

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~redirecting-more-output:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{IW3ceILpE87EM6TDQQqGuO3WH_c.QX1YTN0wSM0AzNzEzW}
```

## What I learned
I learned that we can redirect outputs to other file locations, in this case we use the '>' operator coupled with the execution command to do the same. After this, we can use the command 'cat' to output it from the new location.

## References
Nil.

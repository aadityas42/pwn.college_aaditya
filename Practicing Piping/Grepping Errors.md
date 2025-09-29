# Grepping Errors
The challenge requires you to redirect the errors of a command to the grep command directly, without storing it in a file.

## My Solve
**Flag:**  'pwn.college{AzM94Y5OOOBFGv5-kmM6W-NnXKS.QX1ATO0wSM0AzNzEzW}'

We execute the '/challenge/run 2>& 1 | grep pwn.college' command to redirect the errors from the 'run' program directly into the grep command, without needing to store it in a file, because of the pipe '|' operator.

```
hacker@piping~grepping-errors:~$ /challenge/run 2>& 1 | grep pwn.college
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge checks for a specific process at the other end of stderr : grep
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stderr to another process. Checking...
[TEST] Performing checks on that process!

[INFO] The process' executable is /nix/store/8b4vn1iyn6kqiisjvlmv67d1c0p3j6wj-gnugrep-3.11/bin/grep.
[INFO] This might be different than expected because of symbolic links (for example, from /usr/bin/python to /usr/bin/python3 to /usr/bin/python3.8).
[INFO] To pass the checks, the executable must be grep.

[PASS] You have passed the checks on the process on the other end of my stderr!
[PASS] Success! You have satisfied all execution requirements.
pwn.college{AzM94Y5OOOBFGv5-kmM6W-NnXKS.QX1ATO0wSM0AzNzEzW}
```

## What I learned
I learned how to use redirection of errors without the need to store them in any file, by using the pipe '|' operator. 
I also learned that this is done using the '2>& 1' operator, which is basically a two step process of redirecting the standard error to standard output, and then pipe the now combined standard error and standard output normally as a whole.

## References
Nil.

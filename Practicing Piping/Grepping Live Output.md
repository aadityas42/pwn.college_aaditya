# Grepping Live Output
The challenge requires you to redirect the output of a command to the grep command directly, without storing it in a file.

## My Solve
**Flag:**  'pwn.college{kr2Plo6oXcP_dcBH1s7Ivw3q0JB.QX5EDO0wSM0AzNzEzW}'

We execute the '/challenge/run | grep pwn.college' command to redirect the output from the 'run' program directly into the grep command, without needing to store it in a file, because of the pipe '|' operator.

```
hacker@piping~grepping-live-output:~$ /challenge/run | grep pwn.college
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge checks for a specific process at the other end of stdout : grep
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stdout to another process. Checking...
[TEST] Performing checks on that process!

[INFO] The process' executable is /nix/store/8b4vn1iyn6kqiisjvlmv67d1c0p3j6wj-gnugrep-3.11/bin/grep.
[INFO] This might be different than expected because of symbolic links (for example, from /usr/bin/python to /usr/bin/python3 to /usr/bin/python3.8).
[INFO] To pass the checks, the executable must be grep.

[PASS] You have passed the checks on the process on the other end of my stdout!
[PASS] Success! You have satisfied all execution requirements.
pwn.college{kr2Plo6oXcP_dcBH1s7Ivw3q0JB.QX5EDO0wSM0AzNzEzW}
```

## What I learned
I learned how to use redirection without the need to store the result in any file, by using the pipe '|' operator. This eliminates the middleman that is the file. 
The pipe operator basically links or 'pipes' the output from the program to the left of the operator to that to the right.

## References
Nil.

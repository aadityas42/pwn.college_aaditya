# Grepping Stored Results
The challenge requires you to redirect the output of a command to a file and then grep that file for the flag.

## My Solve
**Flag:**  'pwn.college{Y_fz8BesJSJvW8DTkug_-tnT4YS.QX4EDO0wSM0AzNzEzW}'

We execute the '/challenge/run > /tmp/data.txt' command which redirects the output of the program to the data.txt file, which now contains a hundred thousand lines to text. 
To find the flag in this, we use the grep command with 'pwn.college' as the argument since we know that all fllags start with that argument.

```
hacker@piping~grepping-stored-results:~$ /challenge/run > /tmp/data.txt
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : /tmp/data.txt
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stdout to a file called /tmp/data.txt. Checking...

[HINT] File descriptors are inherited from the parent, unless the FD_CLOEXEC is set by the parent on the file descriptor.
[HINT] For security reasons, some programs, such as python, do this by default in certain cases. Be careful if you are
[HINT] creating and trying to pass in FDs in python.

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~grepping-stored-results:~$ grep pwn.college  /tmp/data.txt
pwn.college{Y_fz8BesJSJvW8DTkug_-tnT4YS.QX4EDO0wSM0AzNzEzW}
```

## What I learned
I learned how to use redirection coupled with other commands, in this case, grep. This is useful as it opens up lots of new possibilities and potential for interesting outcomes.

## References
https://www.reddit.com/r/linuxquestions/comments/vfwcdm/grep_command_error/
I had to refer this because at first I tried to use the grep command with the '-name' argument for grep which was giving me an 'invalid max count' error. Later I realised that the '-name' argument isn't necessary so I executed the command without it.

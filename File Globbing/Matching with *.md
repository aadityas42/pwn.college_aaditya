# Matching with *
The challenge requires you to use file globbing.

## My Solve
**Flag:**  'pwn.college{wir2Paxi-yU1bElU6q7trtFBQRP.QXxIDO0wSM0AzNzEzW}'

We execute the 'cd /c*' command as we have a limit of passing only 4 charecters and the '*' matches any pattern, and the only pattern here to complete the command would be 'challenge' so we can switch our cwd without entering the full command.

```
hacker@globbing~matching-with-:~$ cd /c*
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{wir2Paxi-yU1bElU6q7trtFBQRP.QXxIDO0wSM0AzNzEzW}
```

## What I learned
I learned how carry out the functions of commands without entering the entire command, by using file globbing.
I learnt that file globbing completes the remaining part of the command with any pattern that matches. If there are multiple patterns that match, it displays all the options, and if none match the pattern, it leaves the glob command unchanged. The glob also cannot match a '/' or a leading '.'.

## References
Nil.

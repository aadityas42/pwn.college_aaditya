# Tab Completion for Commands
The challenge requires you to use tab completion for commands to get the flag.

## My Solve
**Flag:**  'pwn.college{wVbB9ZpuK2v939RtXc3OrzSwG2D.0VN0EzNxwSM0AzNzEzW}'

All we need to do for this challenge is enter 'pwncollege' and hit tab, then the autocomplete for commands does the rest of the work, and we obtain the flag.

```
hacker@globbing~tab-completion-on-commands:~$ pwncollege-27843 
Correct! Here is your flag:
pwn.college{wVbB9ZpuK2v939RtXc3OrzSwG2D.0VN0EzNxwSM0AzNzEzW}
```

## What I learned
I learned that tab completion works not only for files, but also for commands, as such, I learned how to implement this in the shell, which can save a lot of time.

## References
Nil.

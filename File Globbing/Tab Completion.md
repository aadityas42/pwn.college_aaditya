# Tab Completion
The challenge requires you to use tab completion to obtain the flag.

## My Solve
**Flag:**  'pwn.college{soo3vQWBdHxcyuP4prXy90BU-ws.0FN0EzNxwSM0AzNzEzW}'

First, we enter 'cat /challenge/pwn' and then hit the 'tab' key, which auto completes 'pwn' to 'pwncollege', giving us the flag.
```
hacker@globbing~tab-completion:~$ cat /challenge/pwncollege​ 
pwn.college{soo3vQWBdHxcyuP4prXy90BU-ws.0FN0EzNxwSM0AzNzEzW}
```

## What I learned
I learned that although using '*' to autocomplete commands may be tempting, it's not always the best choice since it can lead to mismatches and result in unwanted files being included.
As such, it is more preferrable to us 'tab completion', and simply hit 'tab' to autocomplete our commands.

## References
Nil.

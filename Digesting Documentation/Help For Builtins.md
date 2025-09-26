# Help for Builtins
The challenge requires you to read the help page for a builtin command to get the flag.

## My Solve
**Flag:**  'pwn.college{AE8y5xg5FWE3FJFQmF_u9UQzBIR.QX0ETO0wSM0AzNzEzW}'

First we execute the 'help challenge' command to read the help page for the challenge command which tells us that the argument we need is '--secret AE8y5xg5'  and we can get the flag from that.

```
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!
    
    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "AE8y5xg5".
hacker@man~help-for-builtins:~$ challenge --secret AE8y5xg5
Correct! Here is your flag!
pwn.college{AE8y5xg5FWE3FJFQmF_u9UQzBIR.QX0ETO0wSM0AzNzEzW}
```

## What I learned
I learned that the builtin commands like 'cd' , 'ls' and so on also have help pages which can be accessed by 'help builtin_name' which can give us important information on the builtins.
I also learned that the builtins are handelled internally by the shell rather than being invoked as a seperate program.

## References
Nil.

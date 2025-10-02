# Deleting Newlines
The challenge requires you to delete the newlines that have been inserted into the flag.

## My Solve
**Flag:**  'pwn.college{4fQNrgalGGr4-1vQnjY7k0Fsx8u.0VNxEzNxwSM0AzNzEzW}'

To fix our flag, we can use the 'tr -d "\n" command which will delete all newlines represented by "\n" from our flag, giving us the corrected flag.

```
hacker@data~deleting-newlines:~$ /challenge/run | tr -d "\n"
Your line-split flag: pwn.college{4fQNrgalGGr4-1vQnjY7k0Fsx8u.0VNxEzNxwSM0AzNzEzW}
```

## What I learned
I learned that the '\n' operator can be used as a line seperator and must be used in quotes "" to prevent the shell from interpreting it incorrectly and passing it into the tr command.
If we want to delete the '\' operator, we must use it as '\\' since the shell will interpret it as a single '\'.
I learned that the 'tr' command also be used to delete newlines(\n) 
We can use this to convert a stream of data into a single line to better evaluate it.

## References
Nil.

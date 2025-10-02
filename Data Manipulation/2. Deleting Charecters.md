# Deleting Charecters
The challenge requires you to delete certain given charecters from the flag while printing it.

## My Solve
**Flag:**  'pwn.college{Eqcoaiwirxef0sslvw1BPxRmiw8.0FNxEzNxwSM0AzNzEzW}'

To fix our charecter-stuffed flag, we use the 'tr -d ^%' command which uses the '-d' flag to delete the '^' and '%' charecters from the flag, which gives us the actual flag.

```
hacker@data~deleting-characters:~$ /challenge/run | tr -d ^%
Your character-stuffed flag:
pwn.college{Eqcoaiwirxef0sslvw1BPxRmiw8.0FNxEzNxwSM0AzNzEzW}
```

## What I learned
I learned that the 'tr' command also be used to delete charecters or  basically translate them to "nothing". 
This can be done using the '-d' flag' followed by an argument of the charecters we wish to delete. 
This is very useful for eliminating trash/garbage values from within a useful quantity.

## References
Nil.

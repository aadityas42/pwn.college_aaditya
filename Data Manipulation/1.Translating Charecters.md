# Translating Charecters
The challenge requires you to correct the case-swapped flag that is printed.

## My Solve
**Flag:**  'pwn.college{Aj3g64zRQCxqD2JGHj5qPmxd_It.01MxEzNxwSM0AzNzEzW}'

To fix our case-swapped flag, we can use the 'tr' translate command and have it take the first argument as all charecters first capitalised and then small, followed by the reverse as the second argument, this will successfully case-swap our flag back to it's original/correct state.

```
hacker@data~translating-characters:~$ /challenge/run | tr ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz abcdefghijklmnopqrstuvwxyzABCDEFGHI
JKLMNOPQRSTUVWXYZ
yOUR CASE-SWAPPED FLAG:
pwn.college{Aj3g64zRQCxqD2JGHj5qPmxd_It.01MxEzNxwSM0AzNzEzW}
```

## What I learned
I learned how to use the translate command 'tr' which can be used in scenarios like that of our challenge, where we have to swap certain charecters with others, since the main aim of pipin data is to change it, this can prove to be very useful.
The 'tr' command takes the charecters in it's first argument and swaps them with those in it's second argument.

## References
Nil.

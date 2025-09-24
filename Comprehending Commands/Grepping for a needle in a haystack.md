# Grepping for a needle in a haystack
The challenge requires you to use the 'grep' command to search for a particular string in a given file with a hundred thousand lines of text.

## My Solve
**Flag:**  'pwn.college{UnFoTOr6oeN_0raR-X8trFZTtAR.QX3EDO0wSM0AzNzEzW}'

I used the 'grep' command with 'pwn.college' as the argument since we are in search of the flag, which always starts with 'pwn.college', and I used the '/challenge/data.txt' as the directory as that is where we are told the flag is hidden in the hundred thousand lines of text.

```
hacker@commands~grepping-for-a-needle-in-a-haystack:~$ grep pwn.college /challenge/data.txt
pwn.college{UnFoTOr6oeN_0raR-X8trFZTtAR.QX3EDO0wSM0AzNzEzW}
```

## What I learned
I learned that that the grep command proves to be an essential tool while looking for a string of contents that we need when the file size is too large for us to cat it and be able to search it efficiently, like in this case where we have a hundred thousand lines of text, it is like searching for a needle in a haystack.
I also learned that the grep command achieves this by searching for strings containing the argument we give it, and prints all of those strings which have the argument.

## References
Nil.

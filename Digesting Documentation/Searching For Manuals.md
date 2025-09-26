# Searching For Manuals
The challenge requires you to search for a manual using instructons from another manual which has the argument rquired to print the flag.

## My Solve
**Flag:**  'pwn.college{UtFnInkltSo8w4Q63kjpmMcSe3v.QX2EDO0wSM0AzNzEzW}'

First we execute the 'man challenge' command to open the manual, and from there we learn that we need to use 'man -k challenge' next and so we use that and command to get know of 'tnnkltowkj' as the next manual. From there, we get the argument '--tnnklt 846' to print our flag.

```
hacker@man~searching-for-manuals:~$ man challenge
hacker@man~searching-for-manuals:~$ man -k challenge
tnnkltowkj (1)       - print the flag!
hacker@man~searching-for-manuals:~$ man tnnkltowkj
hacker@man~searching-for-manuals:~$ /challenge/challenge --tnnklt 846
Correct usage! Your flag: pwn.college{UtFnInkltSo8w4Q63kjpmMcSe3v.QX2EDO0wSM0AzNzEzW}
```

## What I learned
I learned how to navigate complex manuals that nested one inside another and to extrapolate useful data from them.

## References
Nil.

# Moving Files
The challenge requires you to use the 'mv' command to move files around.

## My Solve
**Flag:**  'pwn.college{gHT1fYcpa5PomVB-Xj-emGyea0V.0VOxEzNxwSM0AzNzEzW}'

First, I used the 'mv' flag to move the flag from the 'flag' file to the 'hack-the-planet!' file located in the 'tmp' directory, after which i run the checker to ensure the flag has moved and is obtained.

```
hacker@commands~moving-files:~$ mv /flag /tmp/hack-the-planet
Correct! Performing 'mv /flag /tmp/hack-the-planet'.
hacker@commands~moving-files:~$ /challenge/check
Congrats! You successfully moved the flag to /tmp/hack-the-planet! Here it is:
pwn.college{gHT1fYcpa5PomVB-Xj-emGyea0V.0VOxEzNxwSM0AzNzEzW}
```

## What I learned
I learned how to move the contents of files about in Linux which is much simpler and faster than deleting and creating the files again to acheive the same thing.


## References
Nil.

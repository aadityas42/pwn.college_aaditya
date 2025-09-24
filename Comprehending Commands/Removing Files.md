# Removing Files
The challenge requires you to use the 'rm' command to delete a file.

## My Solve
**Flag:**  'pwn.college{UXCPPpzGl9mCwLwGTVciAbGJWgj.QX2kDM1wSM0AzNzEzW}'

First, I used the 'ls' command to list out the files present, then used the 'rm delete_me' command to delete the 'delete_me' file from our home directory as specified.

```
hacker@commands~removing-files:~$ ls
a  delete_me
hacker@commands~removing-files:~$ rm delete_me
hacker@commands~removing-files:~$ /challenge/check
Excellent removal. Here is your reward:
pwn.college{UXCPPpzGl9mCwLwGTVciAbGJWgj.QX2kDM1wSM0AzNzEzW}
```

## What I learned
I learned how to delete files on Linux, because at one point or another, we have too many files and need to get rid of them, so it's an essential tool to learn.


## References
Nil.

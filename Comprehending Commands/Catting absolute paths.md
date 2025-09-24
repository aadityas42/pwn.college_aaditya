# Catting abolsute paths
The challenge requires you to use the 'cat' command to display the contents of a file on the terminal window.

## My Solve
**Flag:**  'pwn.college{MlkFFRhZi6N7IXJjLJHuRctigdp.QX5ETO0wSM0AzNzEzW}'

I used the 'cat /flag' command to output the contents of the flag file. We are told that the flag is not stored in the home directory so we need to use an absolute path to obtain it so we use '/flag' rather than just 'flag' like we did in the last challenge.

```
hacker@commands~catting-absolute-paths:~$ cat /flag
pwn.college{MlkFFRhZi6N7IXJjLJHuRctigdp.QX5ETO0wSM0AzNzEzW}
```

## What I learned
I learned that that the cat command can be used to read out the contents of a file using an abolsute path as well and that we can use it outside of the home directory as well.
I also learned that the flag files always lives in pwn.college but in the other challenges, we can't access it directly.

## References
Nil.

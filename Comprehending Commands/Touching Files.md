# Touching Files
The challenge requires you to use the 'touch' command to create two new files.

## My Solve
**Flag:**  'pwn.college{wfIxop0h92LHDaoqliyLUP-TSuf.QXwMDO0wSM0AzNzEzW}'

First, I used the 'cd /tmp' command to switch my cwd to tmp as the files are to be created inside of this directory.
Next, I used the 'touch' command to create the pwn and college files as specified in the tmp directory.

```
hacker@commands~touching-files:~$ cd /tmp
hacker@commands~touching-files:/tmp$ touch pwn
hacker@commands~touching-files:/tmp$ touch college
hacker@commands~touching-files:/tmp$ /challenge/run
Success! Here is your flag:
pwn.college{wfIxop0h92LHDaoqliyLUP-TSuf.QXwMDO0wSM0AzNzEzW}
```

## What I learned
I learned how to create new empty files using the terminal by "touching" it with the 'touch' command.


## References
Nil.

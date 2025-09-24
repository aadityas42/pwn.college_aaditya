# Hidden Files
The challenge requires you to use the 'ls -a' command to list hidden files and obtain the flag from one of them.

## My Solve
**Flag:**  'pwn.college{YkoJRMZNf-0tHCP46l5mEt6byQ6.QXwUDO0wSM0AzNzEzW}'

First, i use the 'cd /.' to move our cwd to the '.' directory, next I used the 'ls -a' command to list the hidden files.
We can see that one of the files, namely '.flag-1216027273648' is the disguised file which contains the flag. So, i use the cat command to list it's contents to obtain the flag.
```
hacker@commands~hidden-files:~$ cd /.
hacker@commands~hidden-files:/$ ls -a
.   .dockerenv           bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-1216027273648  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:/$ cat .flag-1216027273648
pwn.college{YkoJRMZNf-0tHCP46l5mEt6byQ6.QXwUDO0wSM0AzNzEzW}
```

## What I learned
I learned that the 'ls' command doesn't list all of the files in a directory. Namely, files starting with a '.' aren't listed using the command as a convention in Linux. So, we have to use a varient of the command, which is 'ls -a' to list all of the files, including the hidden ones.


## References
Nil.

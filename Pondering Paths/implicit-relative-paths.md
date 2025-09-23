# Implicit Realtive Paths, from /
The challenge requires you to implement relative path instead of absolute path to invoke a program.

## My Solve
**Flag:**  'pwn.college{oCYMJ50j_8QzqwUc7GnVH8CHVka.QX5QTN0wSM0AzNzEzW}'

First we execute 'cd /' command as the challenge states we must start from the / directory. This is also to learn how to use realtive paths instead of absolute since our next directory won't include a / at the beginning now. So, next I execute 'challenge/run' instead of 'cd /challenge/run' because that is an absolute path, and we have already started with / as our current working directory or cwd.

```
hacker@paths~implicit-relative-paths-from-:~$ cd /
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{oCYMJ50j_8QzqwUc7GnVH8CHVka.QX5QTN0wSM0AzNzEzW}

```

## What I learned
I learned that we can invoke programs using relative directories as well as asbsolute ones.For absolute paths, our cwd, which is where our prompt is currently located, doesn't matter, whereas the relative directory's path is relative to our current working directory and is a directory that doesn't start at the root or with a '/'.
For example: If I want to access a file located at /a/b/c/file, and my current working directory is /a/b, my realtive path to access the file will be c/file.

## References
Nil.

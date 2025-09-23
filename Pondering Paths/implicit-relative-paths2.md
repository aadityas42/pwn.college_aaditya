# Implicit Realtive Paths
The challenge requires you to practise using . in your commands while referring to paths more, requiring us to run it from the '/challenge' directory.

## My Solve
**Flag:**  'pwn.college{QPambEPBh0jD1sgVTYr3gnSdOyT.QXxUTN0wSM0AzNzEzW}'

First we execute 'cd /challenge' command to enter the challenge directory, and then invoke the run program using './rn' because linux prevents us from using 'run' directly as a safety measure.

```
hacker@paths~implicit-relative-path:~$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{QPambEPBh0jD1sgVTYr3gnSdOyT.QXxUTN0wSM0AzNzEzW}

```

## What I learned
I learned that we need to use . in some commands to invoke programs because linux has a safety feature that prevents us from using the naked path directly. If linux scanned the current directory everytime we entered a naked path, it could accidently execute programs in the cwd that have the same name as some core system utilities.

## References
Nil.

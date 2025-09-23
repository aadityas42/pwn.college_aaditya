# Position Elsewhere
The challenge requires you to switch directories using the 'cd' command to execute programs stored in different directories

## My Solve
**Flag:**  'pwn.college{c1_vDettC6cB2ck1J0paJBP0obE.QX3QTN0wSM0AzNzEzW}'

First, I checked which direcotry is the program located in. I found it to be the /etc directory by inspection, so i used 'cd /etc' to switch to this directory and then executed the program by '/challenge/run'.

```
hacker@paths~position-elsewhere:/usr/share/doc$ cd /etc
hacker@paths~position-elsewhere:/etc$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{c1_vDettC6cB2ck1J0paJBP0obE.QX3QTN0wSM0AzNzEzW}

```

## What I learned
I learned how to find a directory that is in the history stored by the shell, and switch to it to execute a program.

## References
Nil.

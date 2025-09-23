# Position Yet Elsewhere
The challenge requires you to switch directories using the 'cd' command to execute programs stored in different directories

## My Solve
**Flag:**  'pwn.college{Qb5Lo8mmmC6jT5PknNVF65P1_Hc.QX4QTN0wSM0AzNzEzW}'

First, I checked which direcotry is the program located in. I found it to be the /var directory inside the /etc directory by inspection, so i used 'cd /etc', followed by 'cd /var'  commands to switch to this directory and then executed the program by '/challenge/run'.

```
hacker@paths~position-yet-elsewhere:~$ cd /etc
hacker@paths~position-yet-elsewhere:/etc$ cd /var
hacker@paths~position-yet-elsewhere:/var$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{Qb5Lo8mmmC6jT5PknNVF65P1_Hc.QX4QTN0wSM0AzNzEzW}

```

## What I learned
I learned how to be more fluent in finding a directory that is stored in the history stored by the shell, and switch to it to execute a program.

## References
Nil.

# Listing Files
The challenge requires you to use the 'ls' command to list contents of a file to run a renamed file.

## My Solve
**Flag:**  'pwn.college{oTL5Rgn2nsO2xugOoDlhe5cKK4m.QX4IDO0wSM0AzNzEzW}'

First, I used the 'ls /challenge' which basically lists the files inside the challenge directory, since the run file has been renamed, we can obtain it's new name this way. And, as we expected, we can see the renamed file '15119-renamed-run-5795' and then we can run the program to get our flag.

```
hacker@commands~listing-files:~$ ls /challenge
15119-renamed-run-5795  DESCRIPTION.md
hacker@commands~listing-files:~$ /challenge/15119-renamed-run-5795
Yahaha, you found me! Here is your flag:
pwn.college{oTL5Rgn2nsO2xugOoDlhe5cKK4m.QX4IDO0wSM0AzNzEzW}
```

## What I learned
I learned how to list the contents of a directory using the 'ls' command which is essential while trying to work with files that may have an updated name, or those whose names we do not know.


## References
Nil.

# Home Sweet Home
The challenge requires us to copy the flag to a directory which we specify, inside our home directory.

## My Solve
**Flag:**  'pwn.college{g0xpKZHoOzXSWIJwW9lI2LAbGss.QXzMDO0wSM0AzNzEzW}'
I used the '/challenge/run ~/a' command to copy the flag to the 'a' directory located in our home directory.

```
hacker@paths~home-sweet-home:~$ /challenge/run ~/a
Writing the file to /home/hacker/a!
... and reading it back to you:
pwn.college{g0xpKZHoOzXSWIJwW9lI2LAbGss.QXzMDO0wSM0AzNzEzW}

```

## What I learned
I learned that the home directory is where most of the files we use are stored, and it is where our shell sessions start. I also learned the ~ operator can be used as a shorthand for our home directory. So, whenever the terminal sees a ~ followed in a way consistent with a path and will expand it to our home directory.
Only the leading ~ is expanded, the other ones are not. For example: if we have ~/~/~ it will be expanded to home/hacker/~/~ instead of 'home/hacker/home/hacker/home/hacker' 
Just using the 'cd' command without any argument switches to our home directory by default 

## References
Nil.

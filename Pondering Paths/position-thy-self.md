# Position thy self
The challenge teaches you to navigate between directories using the 'cd' command

## My Solve
**Flag:**  'pwn.college{YCBdxrI3AVy5WTSUSinub87hCNl.QX2QTN0wSM0AzNzEzW}'
First we use 'cd' to change our directory to the giveen directory /usr/share/doc since that is where the program is located
Then, we execute the '/challenge/run' path as the argument to invoke the program. This works because the name of the program is run which is stored in the challenge directory. 

```

hacker@paths~position-thy-self:~$ cd /usr/share/doc
hacker@paths~position-thy-self:/usr/share/doc$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{YCBdxrI3AVy5WTSUSinub87hCNl.QX2QTN0wSM0AzNzEzW}


```

## What I learned
I learned how to invoke programs that are not necessarily in the same directory as I'm starting with. So, I learned how to siwtch directories to access programs.

## References
Nil.

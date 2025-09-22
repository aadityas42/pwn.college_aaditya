# Intro to Arguments
The challenge requires you to open the terminal on pwn.college and use the 'echo' and 'hello' commands to obtain the flag.

## My Solve
**Flag:**  'pwn.college{kJJzrn6qUdvC7uiDcZ78cuLNXxX.QX4YjM1wSM0AzNzEzW}'

First we execute the 'echo' command. This can take any amount of arguments. If we type 'echo Hello' , 'Hello' is displayed in the terminal. If we type 'echo Hello Hackers!' , 'Hello Hackers!' is displayed in the terminal. The echo command gives the same output in the terminal as we enter for the argument.
Similarly, we can use the hello command to obtain the flag, by typing 'hello hackers'.

```
hacker@hello~intro-to-arguments:~$ echo Hello
Hello
hacker@hello~intro-to-arguments:~$ echo Hello Hackers!
Hello Hackers!
hacker@hello~intro-to-arguments:~$ hello hackers
Success! Here is your flag:
pwn.college{kJJzrn6qUdvC7uiDcZ78cuLNXxX.QX4YjM1wSM0AzNzEzW}
```

## What I learned
I learned that Linux commands can take more than one argument, and how different arugments give different outputs.
I also learned the use of the 'echo' command, which essentially gives an output same as the input argument, just like a print statement.

## References
Nil.

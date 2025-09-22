# Intro to Arguments
The challenge requires you to use the up arrow key to find the flag in the history stored by the terminal.

## My Solve
**Flag:**  'pwn.college{UViz6y5cMKwvNW_IEh9ydD2DR10.0lNzEzNxwSM0AzNzEzW}'

First we execute the 'echo' command. This can take any amount of arguments. If we type 'echo Hello' , 'Hello' is displayed in the terminal. If we type 'echo Hello Hackers!' , 'Hello Hackers!' is displayed in the terminal. The echo command gives the same output in the terminal as we enter for the argument.
Similarly, we can use the hello command to obtain the flag, by typing 'hello hackers'.

```
hello
echo Hello
echo Hello Hackers!
hello hackers
whoami
hello 
echo Hello
echo Hello Hackers!
hello hackers
the flag is pwn.college{UViz6y5cMKwvNW_IEh9ydD2DR10.0lNzEzNxwSM0AzNzEzW}

```

## What I learned
I learned that the shell saves a history of every command that you invoke. So we can scroll through these commands and even copy them if necessary since typing from scartch can be annoying sometimes.

## References
Nil.

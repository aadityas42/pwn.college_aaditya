# Cat: not the pet, but the command!
The challenge requires you to use the 'cat' command to display the contents of a file on the terminal window.

## My Solve
**Flag:**  'pwn.college{85kxwaAMZcNjJu9YO6WA-Wc2NOG.QXxcTN0wSM0AzNzEzW}'

I used the 'cat flag' command to output the contents of the flag file. We are told that the flag is stored in the flag file located in our home directory, so this eliminates the need to use the cd command to switch the directory and we can directly using the 'cat' command.

```
hacker@commands~cat-not-the-pet-but-the-command:~$ cat flag
pwn.college{85kxwaAMZcNjJu9YO6WA-Wc2NOG.QXxcTN0wSM0AzNzEzW}

```

## What I learned
I learned that that the cat command can be used to read out the contents of a file. When given multiple arguments, this command concatenates them and gives the output. This is where the word 'cat' originates from, rather than the pet which one hears of more commonly.
I also learned that when we enter just the 'cat' command without any argument, it takes the terminal input and displays it again as the output.

## References
Nil.

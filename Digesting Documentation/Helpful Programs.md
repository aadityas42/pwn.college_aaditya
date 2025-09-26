# Helpful Programs
The challenge requires you to read the help page to get the flag.

## My Solve
**Flag:**  'pwn.college{YdyXem0hZWqFVMM7DF5q8AsDcfk.QX3IDO0wSM0AzNzEzW}'

First we execute the '/challenge/challenge -h' command to read the help page which tells us the command to print the flag, along with the secret value the argument needs.

```
hacker@man~helpful-programs:~$ /challenge/challenge -h
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag
hacker@man~helpful-programs:~$ /challenge/challenge -p
The secret value is: 75
hacker@man~helpful-programs:~$ /challenge/challenge -g 75
Correct usage! Your flag: pwn.college{YdyXem0hZWqFVMM7DF5q8AsDcfk.QX3IDO0wSM0AzNzEzW}


```

## What I learned
I learned that not all programs have a manual.In such cases, we can use the help page which might tell us how to run the program this can be done using '--help' , '-h' or '-?' , 'help' in rare cases and also '/?' although this is more common in windows. 

## References
Nil.

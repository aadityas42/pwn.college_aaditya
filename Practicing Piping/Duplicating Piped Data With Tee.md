# Duolicating Piped Data with Tee
The challenge requires you to use the tee command to get a secret argument and then use that to pipe data to get the flag.

## My Solve
**Flag:**  'pwn.college{MV1KaJ6oJeLZIq7kdUh3Wo42j0N.QXxITO0wSM0AzNzEzW}'

We execute the '/challenge/run | tee pwn | /challenge/college' command to get the instructions for the secret command by following this up with a 'cat pwn'.
Then, we execute '/challenge/pwn --secret MV1KaJ6o | /challenge/college' to pipe the data correctly, and get our flag.

```
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee pwn | /challenge/college
Processing...
WARNING: you are overwriting file pwn with tee's output...
The input to 'college' does not contain the correct secret code! This code 
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the 
output of 'pwn' and figure out what the code needs to be.
hacker@piping~duplicating-piped-data-with-tee:~$ cat pwn
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "MV1KaJ6o"
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret MV1KaJ6o | /challenge/college
Processing...
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{MV1KaJ6oJeLZIq7kdUh3Wo42j0N.QXxITO0wSM0AzNzEzW}
```

## What I learned
I that how to pipe data in complex situations like this, where we need a secret argument to be able to do so successfully.

## References
Nil.
